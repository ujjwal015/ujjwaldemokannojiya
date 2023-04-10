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
        stage('Integration testing'){

            steps{
                sh 'mvn -DiskUnitTests'
            }
        }
    }
}
