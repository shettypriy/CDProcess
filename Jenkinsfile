pipeline {
agent none 
    stages {
      stage('build') {
      steps{
        sh 'mvn clean package'
          }
        }
     stage('Deploy') {
      agent { docker 'tomcat:7' } 
            steps {
                sh 'mvn tomcat7:deploy'
                }
              }
            }
          }
                
      
          
