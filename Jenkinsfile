pipeline {
    agent any
    def tag
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                tag = "git describe --tags --abbrev=1"
            }
        }
    }
}
