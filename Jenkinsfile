pipeline {
    agent any

    stages {
        stage('Build CPP Program') {
            steps {
                sh 'make -f makefile hello_world'
            }
        }
    }
}
