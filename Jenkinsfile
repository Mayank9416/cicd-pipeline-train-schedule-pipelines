pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/Mayank9416/cicd-pipeline-train-schedule-pipelines'
            }
        }

        stage('Build') {
            steps {
                sh './gradlew build --no-daemon'
            }
        }

        stage('Archive Artifact') {
            steps {
                archiveArtifacts(artifacts: 'dist/trainSchedule.zip', fingerprint: true)
            }
        }
    }
}
