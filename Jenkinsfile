pipeline {
    agent any
    stages {
        stage('CPUs') {
            steps {
                sh 'lscpu | grep -m1 CPU\\(s\\):'
            }
        }
        stage('Memory') {
            steps {
                sh'lsmem | grep Total\\ online'
            }
        }
    }
}