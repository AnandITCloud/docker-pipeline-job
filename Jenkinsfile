node {

    checkout scm

    docker.withRegistry('https://hub.docker.com/repositories', 'dockerHub') {

        def customImage = docker.build("dockeraman01/docker-pipeline-job")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
