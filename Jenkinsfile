pipeline {
    agent any
     
    stages {
     stage('SCM Code Checkout') {

            steps {
                set PATH=%PATH%;C:\BrowserDrivers;
                checkout scm 
      } 
  }
        stage('Robot Run Test') {
            steps {

                bat 'robot --variable BROWSER:chrome login_tests'
            }
        }
    }
}  
