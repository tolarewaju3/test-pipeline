pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {

                checkout scm

                sh ''' ls -lhrt '''

                def rootDir = pwd()
                println("Current Directory: " + rootDir)

                echo 'Hello World'

                script {
                    modules.first = load "first.groovy"
                }
            }
        }
    }
}

