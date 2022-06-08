pipeline {
    agent any
    
    stages {
        stage('Build CPP Program') {
            steps {
                echo "building"
            }
        }
      stages('test cmd shell') 
        {
         steps 
         {
            echo 'execute cmd ...'
            bat label: '', script: 'ipconfig  -all'
         }
  
    }
}
