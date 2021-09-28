pipeline {
    agent any
    tools {
        maven 'maven'
    }
   
    stages{
        stage('Build'){
            steps{
                 sh script: 'mvn clean package'
                 archiveArtifacts artifacts: 'target/*.war', onlyIfSuccessful: true
            }
        }
   
    }
}
