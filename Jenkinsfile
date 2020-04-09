pipeline{
    agent any
    stages {
        stage('init') {
            steps {
                echo "Hola!"
            }
        }
        stage('build') {
            steps {
                sh '/.mvnw'
            }
        }
    }
}