pipeline {
    agent any
    
    tools {nodejs "node"}
    
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
                tsc src/main.tsx
                tsc App.tsx
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