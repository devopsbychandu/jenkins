pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                sh(returnStdout: true, script: "git tag --sort version:refname | tail -1").trim()
            }
        }
    }
}
