pipeline {
    agent any
    stages {
        stage('verify k6') {
            steps {
                echo 'k6 version'
                sh 'k6 version'
            }
        }
        stage('run k6 test') {
            steps {
                echo 'Running K6 performance tests...'
                sh 'k6 run loadtests/performance-test.js'
            }
        }
    }
}
