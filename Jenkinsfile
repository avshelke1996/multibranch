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
                sh "chmod 777 index.html"
                sh "docker run -dp 70:80 --name s2 httpd"
                sh "docker cp index.html s2://usr/local/apache2/htdocs"
            }
        }
        stage("deploy"){
            steps{
                echo "deploy"
            }
        }
    }
}
