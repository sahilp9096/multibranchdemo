def statusCode =''
pipeline {
    agent any
  
   
     
    stages {
        stage('Build CPP Program') {
            
            steps {
                script
                {
                  environment
                    {
                        env.PATH=env.PATH+";C:\\Windows\\System32"
                        git url: 'https://github.com/sahilp9096/multibranchdemo.git', branch: 'main'
                        bat 'g++ HelloWorld.cpp -o HelloWorld'
                   
                    }
                    
                  }
                
            }
        }
        
    
     
        stage('Run code') {
            
            steps {
                
                script
                {
                      env.PATH=env.PATH+";C:\\Windows\\System32"
                    
                      statusCode= bat script: "HelloWorld.exe", returnStatus:true
                       
                    
                    
                }
                echo "${statusCode}" 
            }
        }
    
    }
}
