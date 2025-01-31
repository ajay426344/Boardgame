pipeline {
    agent { label 'worker-2' }
     
    tools {
        maven 'mvn3'
        jdk 'jdk17'
    }
    
    stages{
        
        stage (Compile) {
            steps{
            sh "mvn compile"
        }
        }
        stage (Test) {
            steps{
              sh "mvn test"  
            }
            
        }
        stage (package){
            steps{
                sh "mvn package"
            }
        }
        
    }
}
