pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            step {
                checkout scm
                git describe --tags --abbrev=1
            }
        }
    }
}
