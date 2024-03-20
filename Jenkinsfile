pipeline {
    agent { label 'self-hosted' }

    stages {
        stage('SonarQube analysis') {
            steps {
                withSonarQubeEnv('SonarQube10X') {
                    bat 'sonar-scanner'
                }
            }
        }
    }
}
