pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'

                script {
                    modules.first = load "first.groovy"
                }
            }
        }
    }
}

