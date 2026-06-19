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
        stage("Maven Build"){
            steps{
                sh """
                    echo "------------Building Application ----------------"
                    mvn clean package
                    echo "------------Application Build Successfully----------"
                   """
            }
        }
    }
}