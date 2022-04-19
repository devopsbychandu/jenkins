def gitTag = null
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                script {
                    gitTag=sh(returnStdout: true, script: "git tag --contains | head -1").trim()
                    $gitTag
                }
            }
        }
    }
}
