pipeline {
    agent any
    
    stages {
        stage('Build CPP Program') {
            steps {
                echo '${mingw_home}'
                bat 'g++ HelloWorld.cpp -o helloworld'
            }
        }
    }
}
