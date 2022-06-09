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
                script
                {
                    environment {
                        env.PATH = env.PATH + ";c:\\Windows\\System32"
                    
                        def statusCode = bat script: "HelloWorld", returnStatus:true
                        echo "$statusCode"
                    }
                    
                }
                def statusCode = bat script: "HelloWorld", returnStatus:true
                echo "$statusCode"
            }
        }
    
    }
}
