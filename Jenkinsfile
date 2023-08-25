pipeline{
    agent any 
    stages{
        stage('Build'){
            steps{
          sh """
            echo "starting"
            ls
            echo "i am here at " >> workspace/hello.txt
            ls 
            ls workspace 
            echo "hello i am here" >> /tmp/final.txt
            echo "listing under tmp directory"
            ls /tmp
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
            ls
            ls workspace 
            ls /tmp
            echo "${currentBuild.currentResult}"
            echo "${env.BUILD_ID}"
            
            echo "finished"
            """
            }
        }
    }
}
