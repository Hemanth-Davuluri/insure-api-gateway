pipeline{
    agent any

    stages{
        stages("Checkout Code"){
            steps{
                checkout scmGit(branches: [[name: '*/main']],
                extensions: [],
                userRemoteConfigs:[[url:'https://github.com/Hemanth-Davuluri/insure-api-gateway.git']])
            }
        }
    }
}