pipeline{
    agent any

    tools {
  maven 'M2_HOME'
}

    triggers {
  pollSCM '* * * * *'
}

    stages{
        stage('maven packages'){
            steps{
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
            }
      
        }
        stage('maven packages'){
            steps{
                sh 'mvn test'
                
            }
      
        }
        stage('test'){
            steps{
                echo 'test'
              
            }
      
        }
        stage('deploy'){
            steps{
                echo 'deploy'
              
            }
      
        }
    }

}