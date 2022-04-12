pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            step {
                checkout scm
            }
        }
        stage("get the tags") {
            steps {
                git describe --tags --abbrev=1
            }
        }
    }
}
