pipeline {
    agent { 
        dockerContainer {    // Pick up the DockerFile in root repo. And excute every command inside the container
            args '-u root:sudo'  // Run docker run commands with these args
        } 
    }
    stages {        
        stage('Test') { 
            steps {
                sh 'echo Starting Tests'                
            }
        }
    }
    post {
        always{
            sh 'echo Cleaning Docker and Shutting Down Server'
        }
    }
}
