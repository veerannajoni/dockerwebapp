node {

    checkout scm

    docker.withRegistry('https://hub.docker.com/repositories', 'd8cbce35-e28f-4814-83fd-76e7e5a7d082') {

        def customImage = docker.build("miltonc/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
