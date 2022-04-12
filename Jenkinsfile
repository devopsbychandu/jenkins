def tag
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                sh """
                     git describe --tags --abbrev=1
                   """
            }
        }
    }
}
