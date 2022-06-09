pipeline {
    agent any
     
    stages {
        stage('Build CPP Program') {
            steps {
                script
                {
         environment {
             env.PATH = env.PATH + ";c:\\Windows\\System32"
         }
                
                    bat {$path}'g++ HelloWorld.cpp -o HelloWorld'
                }
            }
        }
        
    }
}
