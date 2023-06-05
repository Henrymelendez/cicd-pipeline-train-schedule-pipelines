pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        stage('Test'){
            steps {
                echo 'Testing.....'
                echo 'It worked'
            }
        }
       
    }
}
