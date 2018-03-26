pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
		//def mvnHome = tool 'maven_install'
        bat(/"C:\apache-maven-3.5.3-bin\apache-maven-3.5.3\bin\mvn" -Dmaven.test.failure.ignore clean package/)
      }
    }
    stage('archive and Results') {
      steps {
        junit '**/target/surefire-reports/TEST-*.xml'
        archive 'target/*.jar'
      }
    }
  }
}
