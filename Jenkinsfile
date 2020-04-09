node {
    def app

    stage('build') {
        sh 'chmod 777 mvnw && ./mvnw package'
    }

    stage('Build image') {
        app = docker.build("wilgustavo/pipe:1.0")
    }

    stage('Push image') {
        docker.withRegistry('https://registry.hub.docker.com', 'docker-hub-credentials') {
            app.push("${env.BUILD_NUMBER}")
            app.push("latest")
        }
    }
}