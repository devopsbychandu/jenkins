def latestTag
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                chmod +x gitsync.sh
                sh 'gitsync.sh'
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
