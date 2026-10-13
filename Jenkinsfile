pipeline{
    agent{
        label{
            label "built-in"
            customWorkpace "/mnt/Q1"
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
