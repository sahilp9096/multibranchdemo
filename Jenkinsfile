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
     
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    
   
}
