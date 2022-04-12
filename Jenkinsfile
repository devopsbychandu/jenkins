pipeline {
    agent any
    stages {
        stage {
            steps {
                script {
                    git describe --tags --abbrev=0
                }
            }
        }
    }
}
