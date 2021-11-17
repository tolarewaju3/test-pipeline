pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {

                checkout scm

                sh ''' ls -lhrt '''

                echo 'Hello World'

                script {
                    def rootDir = pwd()
                    modules.first = load "${rootDir}/first.groovy"
                }
            }
        }
    }
}

