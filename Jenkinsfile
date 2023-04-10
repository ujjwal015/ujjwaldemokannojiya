pipeline {

    agent any

    stages{

        stage('Git Checkout'){

            steps{
              git 'https://github.com/ujjwal015/ujjwaldemokannojiya.git'
            }
        }
        stage('UNIT Testing'){
            
            steps{
                sh 'mvn test'
            }
        }
        stage('Static code analysis'){
            steps{
                withSonarQubeEnv(credentialsId: 'sonar-api') {
                 sh 'mvn clean package sonar:sonar'
            }
        }
    }
}
