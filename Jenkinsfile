pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            step {
                checkout scm
                def tag = "git describe --tags --abbrev=1"
                sh "echo ${tag}"
            }
        }
    }
}
