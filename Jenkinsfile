pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
				
                sh './my-app npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test '
            }
        }
        
   
        }
        stage('Prod') {
            steps {
                
                sh 'npm start'
            }
        }
    }
}
