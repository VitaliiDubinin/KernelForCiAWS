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

      stage('Deploy'){
      if(env.BRANCH_NAME == 'master'){
        sh 'docker build -t react-app --no-cache .'
        sh 'docker tag react-app localhost:5000/react-app'
        sh 'docker push localhost:5000/react-app'
        sh 'docker rmi -f react-app localhost:5000/react-app'
      }
    }

   }
}