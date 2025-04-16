pipeline{
  agent any
  stages{
    stage('print info'){
      steps{
        sh """
        echo "${env.JOB_NAME}"
        echo "${env.BUILD_ID}"
        pwd
        whoami
        uptime
        echo "${env.HOSTNAME}"
        """
      }
    }
  }
}
