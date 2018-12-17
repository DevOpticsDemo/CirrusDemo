pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        qqwriteFile file: "application.sh", text: "echo Built ${BUILD_ID} of ${JOB_NAME}"
        archiveArtifacts artifacts: '*.sh', fingerprint: true
      }
    }
  }
}
