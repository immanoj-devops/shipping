// pipeline {
//     agent any
//     stages {

//     stage('Maven Compile') {
//             steps {
//                sh "mvn compile"
//             }
//         }
//         stage('Sonar Scan') {
//             steps {
//                sh '''

//                 mvn sonar:sonar \
//                 -Dsonar.projectKey=shipping \
//                 -Dsonar.host.url=http://172.31.74.214:9000 \
//                 -Dsonar.login=7e6f032ffaf3e53f3a3f5e917575ffaad2993620
//                '''
//             }
//         }
//     }
// }

@Library('roboshop') _


pipeline {
    agent any 
    stages {
        stage(''){
            steps {
                 environment {
                     GURL = "google.com"
                 }
                    parameters {
                            string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                        }
                script {
                    log.info 'WelcomeManoj MSG=${GURL} and you love ${params.PERSON}'
                    log.warning 'pleasDontTouchPo'
                }
            }
        }
    }
}