pipeline{
    agent{
        docker {
            image 'node:alpine'
        }
    }
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