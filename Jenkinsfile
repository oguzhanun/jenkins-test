pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                sh 'echo this is build stage...'
                withMaven("Maven"){
                    sh 'mvn clean package'
                }
            }
        }
        stage("test"){
            steps{
                sh 'echo this is test stage...'
                withMaven("Maven"){
                    sh 'mvn test'
                }
            }
        }
    }
}