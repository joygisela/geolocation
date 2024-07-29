pipeline{
    
    agent any

   triggers {
  pollSCM('* * * * *')
}

    tools {
  maven 'M2_HOME'
}

    stages{
        stage('maven packages'){
            steps{
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
            }
      
        }
        stage('test'){
            steps{
                sh 'mvn test'
                
            }
      
        }
   
        stage('deploy'){
            steps{
                echo 'deploy'
              
            }
      
        }
    }

}