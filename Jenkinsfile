node {
    def app

    stage('build') {
        sh 'chmod 777 mvnw && ./mvnw package'
    }

    stage('Build image') {
        app = docker.build("wilgustavo/pipe:1.0")
    }

}