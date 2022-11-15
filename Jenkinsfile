pipeline {

    agent any
  
    environment {
        APP_NAME = "NODE_APP"
        APP_ENV  = "DEV"
    }

    stages {
        
        stage('Cleanup Workspace') {
            steps {
                cleanWs()
                sh """
                echo "Cleaned Up Workspace for ${APP_NAME}"
                """
            }
        }

        stage('Code Build') {
            steps {
                sh """
                echo "Building the application"
                """
            }
        }

        stage('test') {
            steps {
                sh """
                echo "Testing the application"
                """
            }
        }
      
      stage('deploy') {
            steps {
                sh """
                echo "Deploying the application"
                """
            }
        }

    }   
}
