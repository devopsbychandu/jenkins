def tag = load "script.groovy"
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
                    tag.tag()
                }               
            }
        }
    }
}
