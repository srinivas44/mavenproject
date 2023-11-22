pipeline {
  agent any
  tools {
       maven 'Maven 3.5.0'
      }
  stages {
    stage ('Build') {
          steps{
                sh script: 'mvn clean package'
                }
          }
        }
   }
 
