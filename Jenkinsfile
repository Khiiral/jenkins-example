pipeline {
    agent any
    stages {
        stage('maven install') {
            steps {
                withMaven(globalMavenSettingsConfig: '', jdk: '', maven: 'Maven3', mavenSettingsConfig: '', traceability: true) {
                    sh 'mvn clean install'
                }
            }
        }
    }
}
