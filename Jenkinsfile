pipeline {
   agent any

   stages {
      stage("build") {
        steps {
           sh 'npm install'
        }
      }

      stage("test") {
        steps {
         echo 'testing our app...'
        }
      }

      stage("deploy") {
        steps {
         echo 'deploying our app...'
        }
      }

   }
}