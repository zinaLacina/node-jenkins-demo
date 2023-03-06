pipeline {
    agent any
    environment {
        ENV_VARIABLE = 'Environment'
    }
    parameters {
        string(description: 'Parameter', name: 'PARAMETER_VARIABLE', defaultValue: 'Parameter')

    }
    
    stages {
        stage('Tests') {
            steps {
                echo 'Building..'
                // sh 'npm install'
                echo 'Testing..'
                // sh 'npm test'
            }
        }
        stage('Build and push docker image') {
            steps {
                echo "Building"
            }
        }
        stage('Deploy to remote docker host') {
            // environment {
            //     DOCKER_HOST_CREDENTIALS = credentials('demo-docker')
            // }
            steps {
                echo "Deploying"
            }
        }
    }
}