pipeline {
    agent { docker { image 'python' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'echo Hello World'
            }
        }
    }
}
