node {

    checkout scm

    docker.withRegistry('https://hub.docker.com/repository/docker/veeranna123/jenkins', 'dockerhub') {

        def customImage = docker.build("miltonc/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
