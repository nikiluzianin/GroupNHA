pipeline {
    agent any
    
    tools {nodejs "node"}
    
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npx tsc'
                // tsc App.tsx
            }
        }
        stage('Test') {
            steps {
              sh "pwd"
              sh 'npm install'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deployed"
            }
        }
    }
}