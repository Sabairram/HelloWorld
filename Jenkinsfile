pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               bat "rmdir /s /q DemoForJenkinsPipelineGitHub"
                bat "git clone https://github.com/Sabairram/HelloWorld.git"
                bat "mvn clean -f DemoForJenkinsPipelineGitHub"
            }
        }
        stage('install') {
            steps {
                bat "mvn install -f DemoForJenkinsPipelineGitHub"
            }
        }
        stage('test') {
            steps {
                bat "mvn test -f DemoForJenkinsPipelineGitHub"
            }
        }
        stage('package') {
            steps {
                bat "mvn package -f DemoForJenkinsPipelineGitHub"
            }
        }
    }
}
