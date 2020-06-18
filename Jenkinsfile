pipeline {
  agent any
  tools {
       maven 'Maven 3.5'
      }
  stages {
    stage ('Build') {
          steps{
                sh script: 'mvn clean package'
                }
          }
    stage ('Upload .war to Nexus') {
      steps{
             nexusArtifactUploader artifacts: [
                  [artifactId: 'mavenproject',
                   classifier: '',
                   file: 'target/WebProject',
                   type: 'war']
               ], 
               credentialsId: 'Pipeline_Nexus_ID',
               groupId: 'net.systemshub',
               nexusUrl: '192.168.226.150:8081',
               nexusVersion: 'nexus2',
               protocol: 'http',
               repository: 'WebProject_Repo',
               version: '6.0.0'
             }
      
          }
    
        }
   
   }
