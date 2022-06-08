pipeline {
    agent any

    stages {
        stage('Build CPP Program') {
            steps {
                bat 'make -f makefile hello_world'
            }
        }
    }
}
