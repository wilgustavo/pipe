pipeline{
    agent any
    stages {
        def app
        stage('init') {
            steps {
                echo "Hola!"
            }
        }
        stage('build') {
            steps {
                sh 'chmod 777 mvnw && ./mvnw package'
            }
        }
        stage('image') {
            steps {
                app = docker.build("wilgustavo/pipe:1.0")
            }
        }
    }
}