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
                    println("Current Directory: " + rootDir)
                    //modules.first = load "${rootDir}/first.groovy"
                }
            }
        }
    }
}

