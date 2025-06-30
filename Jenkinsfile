pipeline {
    agent any
    stages {
        stage('github checkout code ') {
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/sanjeev0575/Jenkins_pipeline.git'
            }
        }
        stage('maven Test') {
            steps {
                sh 'mvn clean'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
