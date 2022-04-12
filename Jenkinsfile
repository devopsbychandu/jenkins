def tag
pipeline {
    agent any
    stages {
        stage("sourcecodecheckout") {
            steps {
                checkout scm
                chmod +x tag.sh
                ./tag.sh
            }
        }
    }
}
