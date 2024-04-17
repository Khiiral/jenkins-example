pipeline {
    agent any
    stages {
        stage('Log Jenkins maven') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('maven install') {
            steps {
                withMaven(maven: 'Maven3') {
                    sh 'mvn clean install'
                }
            }
        }
    }
}
