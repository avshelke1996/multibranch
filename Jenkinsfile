pipeline{
    agent{
        label{
            label "built-in"
            customWorkpace "/mnt/mainbranch"
        }
    }
    stages{
        stage("clean"){
            steps{
                echo "clean"
            }
        }
        stage("build"){
            steps{
                echo "build"
            }
        }
        stage("deploy"){
            steps{
                echo "deploy"
            }
        }
    }
}
