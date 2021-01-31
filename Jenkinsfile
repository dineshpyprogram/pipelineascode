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

        stage("Build") {
            when {
                //tag "release-*"
                //buildingTag()
                changeRequest()
            }

            steps {
                echo "building release branch"
            }
        }

        stage("changerequest") {
            when {
                changeRequest()
            }
            steps {
                echo "building as there is a PR"
            }
        }
    }
}