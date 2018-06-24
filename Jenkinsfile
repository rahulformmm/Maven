pipeline {
   agent any
    stages {
     stage ('Build') {
      steps {
        git 'https://github.com/rahulformmm/Maven.git'
      }
     }
    
     stage ('Test') {
       steps {
    	sh 'mvn compile'
      }
     }
   
     stage ('Report') {
      Steps {
    	cucumber fileIncludePattern: '**/*.json', sortingMethod: 'ALPHABETICAL'
      }
     }
   }
}


  
