pipeline {
    agent any
    stages {
        stage('CPUs') {
            steps {
                sh 'lscpu | grep -m1 CPU\(s\):'
            }
        }
        stage('Memory') {
            steps {
                sh 'free -g'
            }
        }
        stage('Containers') {
            steps {
                sh 'docker ps'
            }
        }
    }
}