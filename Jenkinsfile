pipeline {
    agent any
    tools {
        maven 'MVN'
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
