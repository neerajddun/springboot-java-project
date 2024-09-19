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
         
    }
}
