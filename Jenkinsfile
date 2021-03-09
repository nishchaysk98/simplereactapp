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
                sh 'npm install'  
            }
        }
        stage('testing'){
            steps{
                sh "npm run test"
            }        
        }
    }
    post {
        success {
            echo "hi"       
        }
    }
}