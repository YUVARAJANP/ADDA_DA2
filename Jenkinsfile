pipeline {
    agent any
    environment {
        // You can remove the PATH configuration, as Jenkins will set it automatically
    }
    tools {
        // Define the Maven tool with the name 'Maven-3.9.4'
        maven 'Maven-3.9.4'
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                script {
                    // Use 'mvn' directly without specifying the full path
                    sh 'mvn clean test'
                }
            }
        }
    }
}
