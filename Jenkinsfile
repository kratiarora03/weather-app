pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Install Node.js dependencies and build the React app
                sh 'npm install && npm run build'
            }
        }
        
        stage('Deploy') {
            steps {
                // Deploy the built React app to your hosting environment
                // Replace the placeholders with your actual deployment commands
                sh 'rsync -avz build/ user@your-server:/path/to/deploy'
            }
        }
    }
}
