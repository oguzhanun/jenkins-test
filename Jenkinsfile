pipeline{
    agent any
    tools{
        maven "Maven"
        jdk "jdk"
    }
    stages{
        stage("build"){
            steps{
                sh 'echo this is build stage...'    
                sh "mvn clean package"
                
            }
        }
        stage("test"){
            steps{
                sh 'echo this is test...'
                sh "mvn test"
            }
        }
    }
}