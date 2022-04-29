 @Library('library@main') _

pipeline {
    agent any

    stages {
       stage('python exec'){
       steps {
       script{
        //this.findFiles('/resources/main.py')
        sh 'echo hello'
        sh 'ls -la'
        sh 'ls  -la ~/'
        sh 'cd ..'
        sh 'ls -la'
        sh 'ls  -la ~/'
       //string cmd= this.libraryResource('~/resources/main.py')
     //  sh 'python cmd'

       //CommandInterface cmd = new DisplayMessage()
       //cmd.setSteps(this)
       //cmd.execute()
       }
       }

       }
//         stage('Build') {
//             steps {
//             sh 'java -version'
//             sh '''export MAVEN_HOME=/opt/apache-maven
//             export PATH=$PATH:$MAVEN_HOME/bin
//             mvn --version
//             mvn clean install
//             mvn sonar:sonar'''
//             echo 'building'
//             }
//         }
//         stage('Test') {
//             steps {
//                 echo 'Testing..'
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 echo 'Deploying....'
//             }
//         }
//         stage('reading from library'){
//         environment {
//                         TEST_CREDS = credentials('test')
//                     }
//         steps{
//             displayMessage "cool user"
//             echo 'USER: $TEST_CREDS_USR'
//             echo 'PSWD: $TEST_CREDS_PSW'
//
// //             withCredentials([usernameColonPassword(credentialsId: 'test', variable: 'demouser')]) {
// //               echo "${credentialsId}"
// //             }
//
//             }
 //       }
    }
}