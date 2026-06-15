pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Stage'
            }
        }

        stage('Test') {
            steps {
                echo 'Test Stage'
            }
        }

        stage('Archive') {
            steps {
                writeFile file: 'artifact.txt', text: 'Build Successful'
                archiveArtifacts artifacts: 'artifact.txt'
            }
        }
    }
}
