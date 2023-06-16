pipeline {
    agent any
    stages { 
        stage('checkout SCM') {
            steps {
              sh "git pull https://github.com/srinivas-0/test.git"
            }
        }
        stage('Compile') {
          steps {
            sh "mvn clean compile"
          }
        }
        stage('Test') {
          steps {
            sh "mvn clean test"
          }
        } 
        stage('package') {
          steps {
            sh "mvn clean package"
          }
        } 
    }
}
