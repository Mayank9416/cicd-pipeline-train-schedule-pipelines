pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'train-Schedule.zip'
            
            }
        }
    }
}
