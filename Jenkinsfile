pipeline {
    agent any
    stages {
    /*    stage("Master build") {
            when {
                branch "master"
            }

            steps {
                echo "Building Master branch"
            }
        }

        stage("Dev build") {
            when {
                branch "dev"
            }
            steps {
                echo "Building dev branch"
            }
        }*/

        stage("Buildtag") {
            when {
                //tag "release-*"
                //buildingTag()
                tag "2.0"
            }

            steps {
                echo "building release branch"
            }
        }
    }
}