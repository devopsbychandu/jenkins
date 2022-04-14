def tag
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
            }
        }
        stage("tag") {
            steps {
                script {
                    tag = load "script.groovy"
                    tag.tag()
                }               
            }
        }
    }
}
