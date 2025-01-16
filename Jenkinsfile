pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from GitHub
                git url: 'https://github.com/Alina2619/your-repo.git', credentialsId: 'your-credentials-id'
            }
        }

        stage('Build') {
            steps {
                // Add your build steps here
                echo 'Building...'
                // For example, if you are using Maven:
                // sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                // Add your test steps here
                echo 'Testing...'
                // For example, if you are using Maven:
                // sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Add your deployment steps here
                echo 'Deploying...'
                // For example, if you are using a shell script:
                // sh './deploy.sh'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
