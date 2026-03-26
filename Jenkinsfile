cat > Jenkinsfile <<'EOF'
pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Website pipeline started'
            }
        }

        stage('List Files') {
            steps {
                bat 'dir'
            }
        }

        stage('Check Website Files') {
            steps {
                bat 'if not exist index.html exit 1'
                bat 'if not exist style.css exit 1'
                echo 'Website files found successfully'
            }
        }

        stage('Show HTML') {
            steps {
                bat 'type index.html'
            }
        }

        stage('Finish') {
            steps {
                echo 'Website pipeline completed successfully'
            }
        }
    }
}
EOF
