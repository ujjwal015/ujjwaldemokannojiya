pipeline {

    agent any

    stages{

        stage('Git Checkout'){

            steps{
              git 'https://github.com/ujjwal015/ujjwaldemokannojiya.git'
            }
        }
        stages('UNIT Testing'){
            
            steps{
                sh 'mvn test'
            }
        }
    }
}
