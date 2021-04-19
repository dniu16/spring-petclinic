pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''mvn clean package
./mvnw package'''
      }
    }

    stage('Run') {
      steps {
        ansiblePlaybook 'pbook.yaml'
      }
    }

  }
}