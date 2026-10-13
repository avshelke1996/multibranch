pipeline{
    agent{
        label{
            label "built-in"
            customWorkspace "/mnt/Q1"
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
                sh "docker run -dp 60:80 --name s3 httpd"
                sh "docker cp index.html s3:/usr/local/apache2/htdocs"
            }
        }
        stage("deploy"){
            steps{
                echo "deploy"
            }
        }
    }
}
