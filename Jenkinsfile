pipeline {
    agent any
    stages {
        stage {
            steps {
                git describe --tags --abbrev=1
            }
        }
    }
}
