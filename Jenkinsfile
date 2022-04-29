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
            withCredentials([usernameColonPassword(credentialsId: 'test', variable: 'demouser')]) {
              echo "${credentialsId}"
            }
            environment {
                JBOSS_CREDS = credentials('test')
                echo "${JBOSS_CREDS}"
            }
            }
        }
    }
}