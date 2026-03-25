pipeline {
    agent any

    stages {
        stage('Checkout Info') {
            steps {
                echo 'Jenkins is running the pipeline.'
                bat 'git --version'
            }
        }

        stage('Read Project File') {
            steps {
                bat 'type notes.txt'
            }
        }

        stage('Success') {
            steps {
                echo 'Build completed successfully.'
            }
        }
    }
}
