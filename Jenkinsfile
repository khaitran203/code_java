pipeline {
    agent any
   

    stages {
        stage('Build') {
            steps {
                echo 'Building.....'
                sh "chmod +x hello.sh"
                sh "./hello.sh"
            }
        }

        stage('Test') {
            when {
                changeset '**/*.sh'
            }
            steps {
                echo 'Testing.....'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying.....'
            }
        }
    }
}
