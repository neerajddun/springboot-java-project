pipeline {
    agent any 

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

        stage ('Integration test ') {

            steps {

                sh 'mvn  verify'
            }
        }
    }
}