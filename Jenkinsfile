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
                    output=bat 'HelloWorld'
                        echo ${output}
                    }
                }
            }
        }
    
    }
}
