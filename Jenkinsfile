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
                // script {
                //     def containerId = sh(
                //         script: 'docker ps -q --latest',
                //         returnStdout: true
                //     ).trim()

                //     echo "Container ID: ${containerId}"

                //     sh "docker kill ${containerId}"
                // }
            }
        }
        stage("build"){
             steps{
                echo "build"
                sh "chmod 777 index.html"
                sh 'docker run -d -p 8080:80 httpd'
                script {
                    def containerId = sh(
                        script: 'docker ps -q --latest',
                        returnStdout: true
                    ).trim()

                    echo "Container ID: ${containerId}"

                    sh "docker cp index.html ${containerId}:/usr/local/apache2/htdocs/index.html"
                }
            }
        }
        stage("deploy"){
            steps{
                echo "deploy"
            }
        }
    }
}
