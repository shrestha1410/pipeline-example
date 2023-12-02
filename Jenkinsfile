pipeline{
    agent any
    stages{
        stage("complie"){
            steps{
                 sh "javac Test.java"
            }
          
        }
        stage("run"){
            steps{
                sh "java Test"
            }
        }
    }
}