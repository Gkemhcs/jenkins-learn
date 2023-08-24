pipeline{
    agent any 
    stages{
        stage('Build'){
            steps{
          sh """
            echo "starting"
            echo "building" 
            echo "finished"
            """
            }
         
        }
        stage("test"){
            steps{
                sh """
            echo "starting"
            echo "testing" 
            echo "finished"
            """
            }
        }
    }
}
