def latestTag
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                script {
                    latestTag = sh(returnStdout:  true, script: "git tag --sort=-creatordate | head -n 1").trim()
                    env.BUILD_VERSION = latestTag
                    echo "env-BUILD_VERSION"
                    // echo "${env.BUILD_VERSION}"
                    echo latestTag
                }
            }
        }
    }
}
