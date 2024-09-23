pipeline {   
    agent any 
    tools{
        jdk 'jdk11'
        maven 'mvn'
    }

    stages {
        stage('Git checkout') {
            steps {
               git branch: 'main', url: 'https://github.com/neerajddun/springboot-java-poject.git'
            }
        }

         stage('Build') {
            steps {
                // Compile the code
                sh 'mvn clean compile'
            }
        }

        stage('Unit Test') {
            steps {
               sh "mvn test"
            }
        }
        stage ('Integration Test') {
            steps {
                sh 'mvn verify'
            }
        }

         
    }
}
