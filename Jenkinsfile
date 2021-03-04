pipeline {
    agent any
     
    stages {
     stage('SCM Code Checkout') {

            steps {
                checkout scm 
      } 
  }
        stage('Robot Run Test') {
            steps {
sh 'export PATH="/home/dell/Desktop/Jenkins-CI-Introduction/BrowserDrivers:$PATH"'
                sh 'robot --variable BROWSER:FireFox login_tests'
            }
        }
    }
}  
