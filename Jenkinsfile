pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                git describe --tags --abbrev=1
            }
        }
    }
}
