pipeline {
    agent any

    stages {
     

        stage('Build') {
            steps {
                // Add build commands here if needed
                echo 'Building the project'
              bat 'docker build -t sample9 .'
            }
        }
         stage('Run Tests') {
            steps {
                // Run tests using Mocha (Windows command)
                echo "testing"
              bat 'docker run -d -p 127.0.0.1:3000:3000 sample9'
            }
        }

        stage('Deploy') {
            steps {
                // Optional: Add your deployment steps (e.g., upload to server, Docker, etc.)
                echo 'Deploying the application'
            }
        }
    }

   
}
