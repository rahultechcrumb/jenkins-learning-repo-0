pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/rahultechcrumb/jenkins-learning-repo-0'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Building project'
            }
        }

        stage('Test') {
            steps {
                sh '''
                chmod +x test.sh
                ./test.sh
                '''
            }
        }

    }
}
