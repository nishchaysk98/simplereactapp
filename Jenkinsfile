pipeline{
    agent{
        docker {
            image 'node:alpine'
        }
    }
    stages{ 
        stage('testing'){
            steps{
                sh "npm run test"
            }        
        }
    }
}