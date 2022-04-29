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
                        test_creds = credentials('test')
                    }
        steps{
            displayMessage "cool user"
            echo "${test_creds}"

//             withCredentials([usernameColonPassword(credentialsId: 'test', variable: 'demouser')]) {
//               echo "${credentialsId}"
//             }

            }
        }
    }
}