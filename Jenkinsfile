pipeline {
    agent { docker { image 'renvissvnce/test' } }
      stages {
        stage('generate password') {
            docker.image('renvissvnce/test').withRun('--help')
    }
  }
}
