pipeline {
    agent {
        docker { image 'renvissvnce/test' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'input.py -h'
            }
        }
    }
}
