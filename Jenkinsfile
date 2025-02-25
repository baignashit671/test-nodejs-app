pipeline { 
   agent any

   tools {
      nodejs 'NodeJS-18' // Ensure this is configured in Jenkins Global Tool Config
   }

   stages {

     stage('Verify Environment') {
        steps {
           sh 'node -v'
           sh 'npm -v'
        }
     }
   
     stage('Install Dependencies') { 
        steps { 
           sh 'npm install' 
        }
     }
     
     stage('Test') { 
        steps { 
           sh 'echo "testing application..."'
        }
      }

     stage("Deploy application") { 
         steps { 
           sh 'echo "deploying application..."'
         }
     }

   }
}
