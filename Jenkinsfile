pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               bat "rmdir  /s /q HelloWorld"
                bat "git clone https://github.com/Sabairram/HelloWorld.git"
                bat "mvn clean -f HelloWorld"
            }
        }
        stage('install') {
            steps {
                bat "mvn install -f HelloWorld"
            }
        }
        stage('test') {
            steps {
                bat "mvn test -f HelloWorld"
            }
        }
        stage('package') {
            steps {
                bat "mvn package -f HelloWorld"
            }
        }
    }
}
