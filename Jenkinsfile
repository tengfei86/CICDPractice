pipeline {
   agent any

   stages {
      stage('Build') {
        steps {
            script {
              echo "LAST_STAGE=$STAGE_NAME"
              echo "gitlabSourceBranch = ${gitlabSourceBranch}   gitlabTargetBranch = ${gitlabTargetBranch}"   
            }
          echo 'Building...'
          echo "Running ${env.BUILD_ID} ${env.BUILD_DISPLAY_NAME} on ${env.NODE_NAME} and JOB ${env.JOB_NAME}"
          echo "${env.gitlabSourceBranch}"
        }
   }
   stage('Test') {
     steps {
        echo 'Testing...'
     }
   }
   stage('Deploy') {
     steps {
       echo 'Deploying...'
     }
   }
  }
}
