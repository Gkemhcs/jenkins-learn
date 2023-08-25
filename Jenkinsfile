pipeline{
    agent any 

    params{
    string(name:"NAME",defaultValue: "GKEMHCS",description:"hello")
        
    }
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
            echo "name is ${NAME}"
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
