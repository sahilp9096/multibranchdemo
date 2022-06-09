pipeline {
    agent any
      environment {
       env.PATH = env.PATH + ";c:\\Windows\\System32"
   }
    stages {
        stage('Build CPP Program') {
            steps {
               bat 'g++ HelloWorld.cpp -o HelloWorld'
            }
        }
        
    }
}
