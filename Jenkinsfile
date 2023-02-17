pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                    sh "g++ demooo.cpp -o ofile"
                    build job: "PES1UG20CS728-1"
                 }
        }
        stage('Test') {
            steps {
                   sh "./ofile"
          }
        }
    }
     post {
            success {
                
                   echo 'pipeline completed'
                }
         failure{
             echo 'Pipeline failed'
         }
        }
}
