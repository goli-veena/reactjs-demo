pipeline {

   agent any

   stages {

     stage('Install Dependencies') {
        steps {
           bat 'npm install'
        }
     }
      stage('packaging application') {
         steps {
           bat 'npm run build'
        }
     }

     stage('Test') {
        steps {
           sh 'echo "testing application..."'
        }
      }

         stage("Deploy npm cloud application") {
         steps {
           sh 'echo "deploying application..."'
         }

     }

        }

   }