pipeline{
    agent any 
    stages{
        stage('Build'){
            steps{
          sh """
            echo "starting"
  
            echo "i am here at " >> workspace/hello.txt
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
            echo "${currentBuild.currentResult}"
            echo "${env.BUILD_ID}"
            
            echo "finished"
            """
            }
        }
    }
}
