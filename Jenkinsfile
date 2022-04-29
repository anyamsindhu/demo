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
        environment {
                        JBOSS_CREDS = credentials('test')
                    }
        steps{
            displayMessage "cool user"
            echo "${JBOSS_CREDS}"

//             withCredentials([usernameColonPassword(credentialsId: 'test', variable: 'demouser')]) {
//               echo "${credentialsId}"
//             }

            }
        }
    }
}