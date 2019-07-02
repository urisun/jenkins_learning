pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh './gradlew clean build'
            }
        }
        stage("Deploy"){
            steps{
                echo 'Deploying to server 2'
            }
        }
    }
    post {
        always {
            junit 'build/reports/'
        }
    }
}