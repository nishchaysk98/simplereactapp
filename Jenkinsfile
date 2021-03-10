pipeline{
    agent{
        docker {
            image 'node:alpine'
        }
    }
    environment {
        CI = 'true' 
    }
    stages{ 
        stage('Build') {
            steps {
                docker.build("my-image")
            }
        }
    }
}