pipeline{
    agent{
        label{
            label "built-in"
            customWorkspace "/mnt/Q2"
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
