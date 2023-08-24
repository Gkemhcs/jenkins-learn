pipeline{
    agent any 
    stages{
        stage('Build'){
            steps{
          sh """
            echo "starting"
            mkdir workspace 
            echo "i am here at " > workspace/hello.txt
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
            echo "${env.BUILD_ID}"
            
            echo "finished"
            """
            }
        }
    }
}
