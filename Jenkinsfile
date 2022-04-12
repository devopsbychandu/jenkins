def tag
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                script {
                    tag = load "script.groovy"
                    tag.tag()
                }
            }
        }
    }
}
