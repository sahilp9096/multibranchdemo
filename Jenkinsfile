pipeline {
    agent any
     
    stages {
        stage('Build CPP Program') {
            steps {
                script
                {
              environment {
             env.PATH = env.PATH + ";c:\\Windows\\System32"
         
                
                    bat 'g++ HelloWorld.cpp -o HelloWorld'
                }
                }
            }
        }
        
    }
    stages {
        stage('run a program') {
            steps {
                script
                {
                    bat 'HelloWorld.exe'
                }
            }
        }
    
}
