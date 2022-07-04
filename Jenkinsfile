node {
    parameters {
        string(
            name: "Length",
            description: "Length of password",
            defaultValue: "12",
        )
    }
        
        stage('Test') {
            docker.image('renvissvnce/test').withRun('--rm ${Length}') { c ->
                    sh "docker logs ${c.id}"
                }
        }
}
