pipeline {
    agent any
    stages {
        stage ("Build my-jar") {
            steps {
                dir ("my-jar") {
                    withMaven() {
                        sh "./mvnw clean deploy"
                    }
                }
            }
        }
        stage ("Build my-war") {
            steps {
                dir ("my-war") {
                    withMaven() {
                        sh "./mvnw clean deploy"
                    }
                }
            }
        }
    }
}