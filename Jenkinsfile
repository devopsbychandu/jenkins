def tag = tag.sh
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                script {
                    sh echo ${tag}
                }
            }
        }
    }
}
