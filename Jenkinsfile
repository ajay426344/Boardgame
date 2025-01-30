pipeline {
    agent {
	label: 'slave-1'
	}
    
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
