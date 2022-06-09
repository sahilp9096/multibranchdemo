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
        
    
     
        stage('Run code') {
            steps {
                def statusCode =' '
                script
                {
                    environment {
                        env.PATH = env.PATH + ";c:\\Windows\\System32"
                    
                        statusCode= bat script: "HelloWorld.exe", returnStatus:true
                       
                    }
                    
                }
               echo "$statusCode" 
            }
        }
    
    }
}
