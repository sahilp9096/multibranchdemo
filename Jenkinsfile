def statusCode =''
pipeline {
    agent any
    environment
    {
        PATH="C:\\Windows\\System32"
   
    }
    stages {
        stage('Build CPP Program') {
            
            steps {
                script
                {

               

                        bat 'g++ HelloWorld.cpp -o HelloWorld'
                   
                
                    
                  }
                
            }
        }
        
    
     
        stage('Run code') {
            
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
