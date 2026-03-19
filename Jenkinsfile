pipeline {
    agent any

    stages {
        stage('full') {
            steps {
                sh 'cat item/output.txt'
            }
        }
        stage ('dir'){
            steps{
               dir('item') {
                     sh 'cat output.txt'
                }
            }
        }
    }
}
