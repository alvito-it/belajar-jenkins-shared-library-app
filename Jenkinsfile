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
                    Output.hello(this, "Groovy")
                }
            }
        }

        stage("Global Variable") {
            steps {
                script {
                    echo(author())
                    echo(author.name())
                    echo(author.channel())
                }
            }
        }

        stage("Parameter") {
            steps {
                script {
                    maven(["clean", "compile", "test"])
                }
            }
        }

        stage("Hello Person") {
            steps {
                script {
                    echo(person([
                        name: "Muhammad Alvito Madisyahputra",
                        age: 22,
                        country: "Indonesia"
                    ]))
                }
            }
        }
    }
}