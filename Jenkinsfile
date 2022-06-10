def statusCode =''
pipeline {
    agent any
    environment
    {
        PATH=""(
                bat(returnStdout: true, script: ';C:\\Windows\\System32')
            )""
    }
    stages {
        stage('Build CPP Program') {
            
            steps {
                script
                {

                       dir('C:\\Users\\Administrator\\AppData\\Local\\Jenkins\\.jenkins\\workspace\\cpp-code-pipelines\\') 
    // some block

                        bat 'g++ HelloWorld.cpp -o HelloWorld'
                   
                    }
                    
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
