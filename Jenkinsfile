pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                sh 'echo this is build stage...'
                withMaven(){
                    sh 'mvn clean package'
                }
            }
        }
        stage("test"){
            steps{
                sh 'echo this is test...'
                withMaven(){
                    sh 'mvn test'

                }
            }
        }
    }
}