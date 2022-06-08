pipeline {
    agent any
    def MINGW_HOME=
    stages {
        stage('Build CPP Program') {
            steps {
                bat 'g++ HelloWorld.cpp -o hello_world'
            }
        }
    }
}
