pipeline {
    agent any
    environment {
        tag = "git describe --tags --abbrev=1"
    }
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                echo $tag
            }
        }
    }
}
