pipeline {
    agent any

    stages {
        stage('Environment Check') {
            steps {
                sh 'java -version'
                sh 'git --version'
            }
        }
        stage('Build') {
            steps {
                echo 'Simulating a build...'
                sh 'touch my-app.build'
            }
        }
        stage('Test') {
            steps {
                echo 'Running a mock health check...'
                sh 'ls -l my-app.build'
            }
        }
    }
    post {
        always {
            echo 'I will always run, regardless of success or failure!'
        }
        success {
            echo 'The build was successful!'
        }
    }
}
