def latestTag
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                script {
                    latestTag = sh(returnStdout:  true, script: "git tag --sort=-creatordate | head -n 1").trim()
                }
            }
        }
        stage("latesttag") {
            steps {
                echo latestTag
            }
        }
    }
}
