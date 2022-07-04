pipeline {
    agent { docker { image 'renvissvnce/test' } }
      stages {
        stage('generate password') {
      steps {
        sh 'docker run -ti renvissvnce/test'
      }
    }
  }
}
