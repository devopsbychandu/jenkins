def gitTag = null
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                script {
                    gitTag=sh(returnStdout: true, script: "git tag --contains | head -1").trim()
                }
            }
        }
        stage('If tagged') {
            when {
                expression {
                    return gitTag;
                }
            }
            steps {
                // ... do something only if there's a tag on this particular commit
            }
        }
    }
}
