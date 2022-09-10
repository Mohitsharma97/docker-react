pipeline { 
  
   agent any

   stages {
   
     stage('Install Dependencies') { 
        steps { 
           sh 'docker build -t mohit/docker-react -f Dockerfile.dev .' 
        }
     }
     
     stage('Test') { 
        steps { 
           sh 'docker run mohit/docker-react npm run test'
        }
      }

         stage("Deploy application") { 
         steps { 
           sh 'echo "deploying application..."'
         }

     }
  
   	}

   }
