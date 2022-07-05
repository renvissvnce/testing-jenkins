node {
    parameters {
        string(
            name: "Name",
            description: "Name of user",
            defaultValue: "lolkek",
        ),
        string(
            name: "Length",
            description: "Length of password",
            defaultValue: "12",
        )
    }
        
        stage('Test') {
            docker.image('renvissvnce/test').withRun('{$Name}: {$Length}') { c ->
                    sh "docker logs ${c.id}"
                }
        }
}
