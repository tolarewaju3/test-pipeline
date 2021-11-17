pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {

                checkout scm

                sh ''' ls -lhrt '''

                echo 'Hello World'

                script {
                    modules.first = load "${rootDir}/first.groovy"
                }
            }
        }
    }
}

