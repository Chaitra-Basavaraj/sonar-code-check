pipeline{
    agent any
    tools{
        maven "test-maven"
    }
    stages{
       stage('GetCode'){
            steps{
                git 'https://github.com/Chaitra-Basavaraj/sonar-code-check.git'
            }
         }        
       stage('Build'){
            steps{
                sh 'mvn clean package'
            }
         }
    }
}
