pipeline {
    agent any
     
    stages {
        stage('Build CPP Program') {
            steps {
         environment {
             env.PATH = env.PATH + ";c:\\Windows\\System32"
   
               bat 'g++ HelloWorld.cpp -o HelloWorld'
            }
            }
        }
        
    }
}
