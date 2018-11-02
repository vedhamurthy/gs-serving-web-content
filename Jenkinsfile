pipeline {
    agent { docker 'gradle:4.5-jdk8-alpine' }
    stages {
	stage('Checkout') {
          steps {
              git 'https://github.com/vedhamurthy/gs-serving-web-content.git'
          }
        }
	stage('Build') {
          steps {
              sh 'gradle clean compileJava'
          }
	}
    }
}
