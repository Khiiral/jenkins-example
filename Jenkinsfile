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
                withMaven(maven: 'maven3') {
                    sh 'mvn clean install'
                }
            }
        }
    }
}
