def statusCode =''
pipeline {
    agent any
   
     
    stages {
        stage('Build CPP Program') {
            environment
                    {
                    env.PATH=env.PATH+";C:\\Windows\\System32"
                    }
            steps {
                script
                {
                  
    
                     bat 'g++ HelloWorld.cpp -o HelloWorld'
                   
                    
                    
                  }
                
            }
        }
        
    
     
        stage('Run code') {
            environment
                    {
                    env.PATH=env.PATH+";C:\\Windows\\System32"
                    }
            steps {
                
                script
                {
                     
                    
                      statusCode= bat script: "HelloWorld.exe", returnStatus:true
                       
                    
                    
                }
                echo "${statusCode}" 
            }
        }
    
    }
}
