pipeline{
    agent any
    environment {
        CI = 'true' 
        dockerImage = ''
    }
    stages{ 
        stage('Build') {
            steps {
                script{
                   dockerImage = docker.build("my-image")
                }
            }
        }
    }
}