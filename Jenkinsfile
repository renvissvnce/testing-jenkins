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
            defaultValue: "12",
        )
    }
    stage('Test') {
        docker.image('renvissvnce/test').withRun { c ->
            sh "--name $NAME --length $LENGTH"
            sh "docker logs ${c.id}"
        }
    }
}
