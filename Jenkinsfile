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
                sh 'robot --variable BROWSER:FireFox login_tests'
            }
        }
    }
}  
