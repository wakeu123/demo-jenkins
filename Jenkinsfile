pipeline{
    agent any
    stages{
        stage('Clone'){
            steps{
                sh "rm -rf *"
                sh "git clone https://github.com/wakeu123/demo-jenkins.git"
            }
        }
        stage('Build'){
            steps{
                sh "cd demo-jenkins/ && javac Hello.java"
                sh "cd demo-jenkins/ && ls"
                sh "cd demo-jenkins/ && java Hello"
            }
        }
    }
}
