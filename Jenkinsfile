pipeline {

    agent any 

    stages {

        stage ('Git Checkout') {

            steps {

                git branch: 'main', url: 'https://github.com/neerajddun/neerajddun-springboot-pipe.git'
            }
        }

        stage ('Unit Test') {

            steps {

              sh 'mvn test'
            }
        }
    }
}