pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/bhumisachdev12/devops-evaluation'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building the project...'
               
              
        }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                  bat 'npm test || echo "No tests defined"'
             
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                 bat 'npm run build' 
               
            }
        }
    }
}
