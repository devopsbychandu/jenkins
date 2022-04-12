pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                sh ./tag.sh
            }
        }
    }
}
