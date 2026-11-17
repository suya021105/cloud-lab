pipeline {
    agent any
    stages {
        stage("Checkout") {
            steps {
                git url: "https://github.com/suya021105/cloud-lab.git", branch: "main"
            }
        }
        stage("Build") {
            steps {
                sh "docker build -t myflask:test ."
            }
        }
    }
}
