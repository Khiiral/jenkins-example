pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                withMaven(maven: 'maven3') {
                    sh 'mvn clean compile'
                }
            }
        }
        stage('Test') {
            steps {
                withMaven(maven: 'maven3') {
                    sh 'mvn test'
                }
            }
        }
        stage('Install') {
            steps {
                withMaven(maven: 'maven3') {
                    sh 'mvn install'
                }
            }
        }
    }
}
