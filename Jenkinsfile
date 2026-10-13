pipeline{
    agent{
        label{
            label "built-in"
            customWorkpace "/mnt/mainbranch"
        }
    }
    stages{
        stage("clean"){
            step{
                echo "clean"
            }
        }
        stage("build"){
            step{
                echo "build"
            }
        }
        stage("deploy"){
            step{
                echo "deploy"
            }
        }
    }
}
