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
                sh "docker run -dp 80:80 --name s1 httpd"
                sh "docker cp index.html s1://usr/local/apache2/htdocs"
            }
        }
        stage("deploy"){
            steps{
                echo "deploy"
            }
        }
    }
}
