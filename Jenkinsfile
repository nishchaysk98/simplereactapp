pipeline{
    agent{
        dockerfile true
    }
    stages{ 
        stage('build for testing purpose'){
            steps{
                sh "docker build -f Dockerfile.dev -t simplereactapp ."
            }        
        }

        stage('build for deployment purpose'){
            steps{
                sh "docker run -e CI=true simplereactapp npm run test"
            }
        }
    }
}