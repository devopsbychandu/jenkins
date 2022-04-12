pipeline {
    agent any
    dev tag
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                tag = "git describe --tags --abbrev=1"
            }
        }
    }
}
