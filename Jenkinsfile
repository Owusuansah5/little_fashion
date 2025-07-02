pipeline {
    agent any

    stages{
        stage('code scan') {
            steps{
                sh 'trivy fs . -o result.html'
                sh 'cat result.html'
                sh 'ls '
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
                sh 'docker images'
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
