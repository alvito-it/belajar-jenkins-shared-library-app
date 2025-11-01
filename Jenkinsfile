@Library("belajar-jenkins-shared-library@main") _

import alvitogamestore.jenkins.Output

pipeline {
    agent any
    stages {
        stage("Hello World") {
            steps {
                script {
                    hello.world()
                }
            }
        }

        stage("Hello Groovy") {
            steps {
                script {
                    Output.hello("Groovy")
                }
            }
        }
    }
}