pipeline{
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('init') {
            steps {
                echo "Hola!"
            }
        }
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}