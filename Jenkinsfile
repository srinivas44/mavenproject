pipeline {
  agent any
  tools {
       maven 'maven'
      }
  stages {
    stage {
          steps{
                sh script: 'mvn clean package'
                }
          }
        }
   
   }

