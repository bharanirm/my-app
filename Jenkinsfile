pipeline {
    agent any

    stages {
         stage('build') {
         def mvnHome=C:\apache-maven-3.5.3-bin\apache-maven-3.5.3
         bat(/"${mvnHome}\bin\mvn" -Dmaven.test.failure.ignore clean package/)
              }
             }
        }
