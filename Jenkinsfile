pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'

                script {
                    modules.first = load "${rootDir}@script/NonCPS.java"
                }
            }
        }
    }
}

