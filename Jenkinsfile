pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               bat "rmdir  /s /q DemoForJenkinsPiplineGitHub"
                bat "git clone https://github.com/Sabairram/HelloWorld.git"
               
            }
        }
        
        }
    }

