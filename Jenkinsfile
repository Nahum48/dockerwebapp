node {
    checkout scm

    docker.withRegistry('https://hub.docker.com', 'dockerHub') {

        def customImage = docker.build("nahum48/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
