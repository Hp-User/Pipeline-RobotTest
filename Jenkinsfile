pipeline {
    agent any
     
    stages {
     stage('SCM Code Checkout') {

            steps {
                 sh 'export PATH=/home/dell/Desktop/Jenkins-CI-Introduction/BrowserDrivers:$PATH'
                checkout scm 
      } 
  }
        stage('Robot Run Test') {
            steps {

                sh 'robot --variable BROWSER:chrome login_tests'
            }
        }
    }
}  
