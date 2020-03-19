node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'credentials-id') {

        def customImage = docker.build("myfirstimage")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
