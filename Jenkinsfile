pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git 'https://github.com/<your-username>/jenkins-ci-demo.git'
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
