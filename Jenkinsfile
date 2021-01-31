pipeline {
    agent any
    stages {
        stage("Run stages in parallel") {
            failFast=true
            stage("stage1") {
                echo "stage1"
                sleep 10
            }
            stage("stage2") {
                echo "stage2"
                sleep 5
            }
            stage("stage3") {
                echo "stage3"
                sleep 5
                error "stage3 errored out"
            }
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
        }

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
        }*/
    }
    }
}