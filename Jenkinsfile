pipeline {
    agent any
     
    stages {
        stage('Build CPP Program') {
            steps {
         environment {
       PATH='c:\Windows\System32'
   }
               bat 'g++ HelloWorld.cpp -o HelloWorld'
            }
        }
        
    }
}
