node {
    parameters {
        string(
            name: "Length",
            description: "Length of password",
            defaultValue: "12",
        )
    }
        
        stage('Test') {
            docker.image('renvissvnce/test').withRun('--rm') { c ->
                    sh "${Length}"
                    sh "docker logs ${c.id}"
                }
        }
}
