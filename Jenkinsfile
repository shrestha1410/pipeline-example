pipeline{
    agent any
    environment{
        VERSION_NAME="1.35"
    }
    stages{
        stage("complie"){
            steps{
                 sh "javac Test.java"
                 sh 'echo "${VERSION_NAME}"'
            }
          
        }
        stage("run"){
            steps{
                sh "java Test"
            }
        }
    }
    post{
        always{
            sh 'echo "always"'

        }
        success{
            sh 'echo "success"'
        }
        failure{
            sh 'echo "failure"'
        }
    }
}