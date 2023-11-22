pipeline {
  agent any
  tools {
       maven 'Maven 3.8.4'
      }
  stages {
    stage ('Build') {
          steps{
                sh script: 'mvn clean package'
                }
          }
        }
   }
 
