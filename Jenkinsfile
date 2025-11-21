pipeline {
    agent any
    tools{
        jdk "jdk17"
        maven "maven3"
    }
    stages {
        stage('Git checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/i-anuj/board-game.git'
            }
        }
        stage('compile') {
            steps {
                sh "mvn compile"
            }
        }
        stage('Build and deploy') {
            steps {
                withMaven(globalMavenSettingsConfig: 'Maven-to-nexus', jdk: 'jdk17', maven: 'maven3', traceability: true) {
                    sh "mvn deploy"
    
                 }
            }
        }
    }
}
