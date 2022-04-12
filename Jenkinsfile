def tag
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                tag = "git describe --tags --abbrev=1"
            }
        }
    }
}
