pipeline {
    agent any
    
    stages {
        stage('Build CPP Program') {
            steps {
                bat 'g++ HelloWorld.cpp -o hello_world'
            }
        }
    }
}
