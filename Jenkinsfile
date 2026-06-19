pipeline {
    agent any

    stages {
        stage("Checkout Code") {
            steps {
                checkout scmGit(branches: [[name: '*/main']],
                    extensions: [],
                    userRemoteConfigs: [[url: 'https://github.com/Hemanth-Davuluri/insure-api-gateway.git']]
                )
            }
        }
    }
}