pipeline {
   agent any

   stages {
      stage("npm install") {
        steps {
            sh 'npm install --save-dev cross-env'
            echo 'npm installed'
        }
      }

      stage("run") {
        steps {
         echo 'npm run done'
        }
      }

    //   stage("deploy") {
    //     steps {
    //      echo 'deploying our app...'
    //     }
    //   }

   }
}