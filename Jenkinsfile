node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/', 'docker-login') {

        def customImage = docker.build("rajeevk7983/nodejs-project")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
