pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "running build step"
                sh './gradlew build --no-daemon'
                arhiveArtifacts artifacts: 'dist/trainSchedule.zip'
                
            }
        }
    }
}
