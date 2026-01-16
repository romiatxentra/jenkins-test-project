pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from the repository...'
            }
        }
        stage('Build') {
            steps {
                echo 'Compiling the application...'
                sh 'mkdir -p build && touch build/app.exe'
            }
        }
        stage('Test') {
            steps {
                echo 'Running automated test...'
                sh 'echo "Test Passed!"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to the "Production" folder...'
                sh 'cp build/app.exe /tmp/deployed_app.exe'
            }
        }
    }
}
