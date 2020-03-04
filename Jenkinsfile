node {
    checkout scm

    docker.withRegistry('https://hub.docker.com', 'dockerhub') {

        def customImage = docker.build("nahum48/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
