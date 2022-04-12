def tag = tag.sh
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            step {
                checkout scm
                script {
                    sh echo ${tag}
                }
            }
        }
    }
}
