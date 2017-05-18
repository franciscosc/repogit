pipeline {
   
   agent any
   
   
   stages{
   
  
   stage('Results') {
          steps { 
              echo "'dddddd'"
          }
   }
  }
    post {
     failure {
         mail to: 'franciscosc@meta4.com',
         subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
         body: "Something is wrong with ${env.BUILD_URL}"
              }
             
   success {
         mail to: 'franciscosc@meta4.com',
         subject: "OK Pipeline: ${currentBuild.fullDisplayName}",
         body: "URL ${env.BUILD_URL}"
              }
      }

   
}