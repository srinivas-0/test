pipeline {
    agent any
    stages { 
        stage('checkout SCM') {
            steps {
              sh "git pull https://github.com/srinivas-0/test.git"
            }
        }
        stage('Test') {
          steps {
            sh "mvn clean package"
          }
        }
        stage('Build') {
          steps {
            sh "mvn clean test"
          }
        } 
    }
}
