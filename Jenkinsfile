pipeline {
    agent any

    parameters {
        booleanParam defaultValue:true, name: 'skip_test'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Hello Build'
            }
        }
        stage('Test') {
            when {expression {params.skip_test!=true}}
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
