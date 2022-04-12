pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                demo=$(git describe --tags --abbrev=0)
                echo $demo
            }
        }
    }
}
