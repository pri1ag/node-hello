node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub') {

        def customImage = docker.build("pri1ag/node-hello")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
