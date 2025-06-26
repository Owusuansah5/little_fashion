pipeline {
    agent any

    stages{
        stage('code scan') {
            steps{
                sh 'trivy --version'
            }
        }
        stage('docker Image build') {
            steps{
                sh 'docker -v'
            }
        }

        stage('push image') {
            steps{
                sh 'docker ps'
            }
        }
        stage('clone') {
            steps{
                sh 'echo "clone"'
                sh 'pwd'

            }
        }
        stage('test') {
            steps{
                sh 'echo "test"'
            }
        }
        stage('create file') {
            steps{
                sh 'touch text-$BUILD_ID'
            }
        }
             
    }
}
