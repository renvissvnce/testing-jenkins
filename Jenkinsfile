pipeline {
    agent {
        docker { image 'renvissvnce/test' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'docker run renvissvnce/test'
            }
            
        }
    }
}
