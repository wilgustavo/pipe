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
                sh 'chmod 777 mvnw && ./mvnw package'
            }
        }
    }
}