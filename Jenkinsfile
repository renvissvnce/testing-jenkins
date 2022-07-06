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
            sh "python input.py -n $NAME -l $LENGTH"
            sh "docker logs ${c.id}"
        }
    }
}
