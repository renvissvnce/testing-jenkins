node {
    parameters {
        string(
            name: "NAME",
            description: "Name of user",
            defaultValue: "lolkek",
        )
        string(
            name: "LENGTH",
            description: "Length of password",
            defaultValue: "15",
        )
    }
    stage('Test') {
        docker.image('renvissvnce/test:latest').withRun(
            "-e test=test",
            "-n $NAME -l $LENGTH") { c ->
            sh "docker logs ${c.id}"
        }
    }
}
