pipeline {
    agent any
 tools {
        jdk 'JDK 17'  // Use the JDK name you configured in Global Tool Configuration
        maven 'Maven'  // If you are using Maven, ensure it is configured too
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