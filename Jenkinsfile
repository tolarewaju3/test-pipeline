pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {

                checkout scm

                sh ''' ls -lhrt '''

                echo 'Hello World'

                sh "wget https://mirror.openshift.com/pub/openshift-v4/clients/oc/latest/linux/oc.tar.gz"
"

                script {
                    def rootDir = pwd()
                    println("Current Directory: " + rootDir)
                    //def example = load "${rootDir}/OpenShiftDSL.groovy"
                    //modules.first = load "${rootDir}/first.groovy"
                }
            }
        }
    }
}

