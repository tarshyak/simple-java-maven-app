pipeline {
    agent any

    tools {
     
        jdk "JDK 9"
        maven "Maven 3"
    }

    stages {
        stage('Build') {
            steps {
            
                
                git 'https://github.com/tarshyak/simple-java-maven-app.git'
                sh "mvn package"
            }

           
            
      post{
        
        success{
          echo "Maven execution successfull"
          
        }
        
      }
        }
        }
    }

