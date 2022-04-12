pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                def tag = "git describe --tags --abbrev=1"
            }
        }
    }
}
