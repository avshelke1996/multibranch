pipeline{
    agent{
        label{
            label "built-in"
            customWorkspace "/mnt/mainbranch"
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
