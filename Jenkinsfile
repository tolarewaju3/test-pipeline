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
                    def example = load "${rootDir}/OpenShiftDSL.groovy"
                    //modules.first = load "${rootDir}/first.groovy"
                }
            }
        }
    }
}

