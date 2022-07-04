node {
    parameters {
        string(
            name: "Length",
            description: "Length of password",
            defaultValue: "12",
        )
    }
        
        stage('Test') {
            docker.image('renvissvnce/test').inside('$Length=12') { c ->
                    sh "docker logs ${c.id}"
                }
        }
}
