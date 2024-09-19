pipeline {   
    agent any 
    tools{
        jdk 'jdk11'
        maven 'mvn'
    }

    stages {
        stage('Git checkout') {
            steps {
                git branch: 'main', changelog: false, poll: false, url: 'https://github.com/jaiswaladi246/springboot-java-poject.git'
            }
        } 
    }
}
