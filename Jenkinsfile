pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "multibranch"
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            
            }
        }
    }
}
