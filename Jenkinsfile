pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               bat "rmdir /s /q DemoForJenkinsPipelineGitHub"
                bat "git clone https://github.com/Sabairram/HelloWorld.git"
               
            }
        }
        
        }
    }

