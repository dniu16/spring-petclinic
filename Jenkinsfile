pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh './mvnw package'
      }
    }

    stage('Run') {
      steps {
        sh 'java -Dserver.port=8888 -jar target/spring-petclinic-2.4.2.jar'
      }
    }

  }
}