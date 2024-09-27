pipeline {
    agent any

    tools {
        maven 'Maven'  // Use the name configured in Jenkins
        jdk 'JDK 17'   // Ensure JDK is also configured in Jenkins
    }

    stages {
        stage('Checkout') {
            steps {
               git branch: 'main', url: 'https://github.com/neerajddun/springboot-java-project1.git'  // Replace with your repository URL
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'  // Build the application
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'           // Run tests
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...' // Add your deployment logic here
            }
        }
    }

    post {
        success {
            echo 'Build and tests succeeded!'
        }
        failure {
            echo 'Build or tests failed.'
        }
    }
}
