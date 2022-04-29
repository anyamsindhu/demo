 @Library('library')_

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'building'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('reading from library'){
        steps{
            displayMessage "cool user"
            }
        }
    }
}