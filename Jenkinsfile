pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {

                checkout scm

                sh ''' ls -lhrt '''

                echo 'Hello World'

                sh 'curl -k -v \
                -X GET  \
                -H "Authorization: Bearer sha256~mYPszAm5BqMgXRMEzaePiNOnTFvqaXZWcgSRJXcQskM" \
                -H "Accept: application/yaml" \
                -H "Content-Type: application/yaml" \
                https://api.sandbox-m2.ll9k.p1.openshiftapps.com:6443/oapi/v1/buildconfigs'

                script {
                    //wget https://mirror.openshift.com/pub/openshift-v4/clients/oc/latest/linux/oc.tar.gz

                    def rootDir = pwd()
                    println("Current Directory: " + rootDir)
                    //def example = load "${rootDir}/OpenShiftDSL.groovy"
                    //modules.first = load "${rootDir}/first.groovy"
                }
            }
        }
    }
}

