 @Library('library')_

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
            sh 'java -version'
            sh '''export MAVEN_HOME=/opt/apache-maven
            export PATH=$PATH:$MAVEN_HOME/bin
            mvn --version
            mvn clean package'''
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
                        TEST_CREDS = credentials('test')
                    }
        steps{
            displayMessage "cool user"
            echo 'USER: $TEST_CREDS_USR'
            echo 'PSWD: $TEST_CREDS_PSW'

//             withCredentials([usernameColonPassword(credentialsId: 'test', variable: 'demouser')]) {
//               echo "${credentialsId}"
//             }

            }
        }
    }
}