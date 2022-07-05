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
        docker.image('renvissvnce/test').inside('${NAME} ${LENGTH}' { c ->
            sh "docker logs ${c.id}"
