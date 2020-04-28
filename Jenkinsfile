pipeline {
    agent any
        stages  {
            stage("Clone Repository") {
                steps {
                    checkout scm
                }
            }
            stage("Build Image") {
                steps {
                    sh 'sudo docker-compose build'
                }
            }
            stage("Run Image") {
                steps {
                    sh 'sudo docker-compose up -d'
                }
            }
        }
}