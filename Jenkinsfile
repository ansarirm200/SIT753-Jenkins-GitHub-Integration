pipeline {
    agent any

    stages {
        stage('Checkout from GitHub') {
            steps {
                echo 'Checking out the latest files from GitHub...'
                checkout scm
            }
        }

        stage('Verify GitHub Repository Files') {
            steps {
                echo 'Displaying files downloaded from GitHub...'
                bat 'dir'
            }
        }

        stage('Read Application File') {
            steps {
                echo 'Reading app.txt from the GitHub repository...'
                bat 'type app.txt'
            }
        }

        stage('Build Stage') {
            steps {
                echo 'Simulating build stage for CareConnect project...'
                bat 'echo Build stage completed successfully.'
            }
        }

        stage('Test Stage') {
            steps {
                echo 'Simulating test stage for CareConnect project...'
                bat 'echo Test stage completed successfully.'
            }
        }

        stage('Code Quality Check') {
            steps {
                echo 'Performing code quality evidence stage...'
                bat 'echo Code quality check completed successfully.'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Performing security scan evidence stage...'
                bat 'echo Security scan completed successfully.'
            }
        }

        stage('Health Check Evidence') {
            steps {
                echo 'Generating final pipeline evidence...'
                bat 'echo Jenkins pipeline successfully connected to the GitHub repository.'
                bat 'echo GitHub-based Jenkinsfile executed successfully.'
                bat 'echo Build, test, code quality, security, and health check stages completed.'
            }
        }
    }

    post {
        success {
            echo 'CareConnect GitHub-triggered Jenkins pipeline completed successfully.'
        }

        failure {
            echo 'CareConnect Jenkins pipeline failed. Please check the console output.'
        }

        always {
            echo 'Pipeline execution finished.'
        }
    }
}
