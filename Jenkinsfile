node {
   
   def fileContent = ''
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/franciscosc/repogit'
     
   }
   stage('Build') {
     fileContent = readFile 'README.md'
   }
   stage('Results') {
      echo "''${fileContent}"
   }
}
