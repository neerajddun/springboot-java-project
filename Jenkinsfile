pipeline {
    agent any

    tools {

        maven 'mvn'
        jdk 'JDK17'
    } 

    stages {

        stage ('Checkout') {

            steps {

                git branch: 'main', url: 'https://github.com/neerajddun/neerajddun-springboot-pipe.git'
            }
        }

        stage ("unit test") {

            steps {

                sh 'mvn test'
            }
        }

    }
}