pipeline {
    agent none 
    stages {
        stage(‘GITCLONE) {
            agent { any} 
            steps {
               
                sh ‘Git clone URL’
            }
        stage(‘GITCLONE) {
            agent { any} 
            steps {
                echo 'Hello, Maven'
                sh 'mvn build . ‘
            }
        }
        stage('Example Test') {
            agent { docker 'openjdk:8-jre' } 
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
