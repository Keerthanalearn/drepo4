pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello Build'
            }
        }
        stage('Test') {
            parallel {                
                stage('Unit test') {
                    steps {
                        echo 'Hello Build'
                    }
                }
                stage('Integration test') {
                    steps {
                        echo 'Hello Build'
                    }
                }
            }
        }
      stage('Deploy') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
