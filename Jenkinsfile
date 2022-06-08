pipeline {
    agent any
    
    stages {
        stage('Build CPP Program') {
            steps {
                echo "building"
            }
        }
          stage('test cmd shell') {
         steps {
            echo 'execute cmd ...'
            bat label: '', script: 'ipconfig  -all'
         }
  
    }
}
