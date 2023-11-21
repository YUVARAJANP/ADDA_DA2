pipeline {
    agent any
    environment {
        // Use a general Maven tool
        M2_HOME = tool 'Maven-3.9.4'
        PATH = "${M2_HOME}/bin:$PATH"
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Use the 'mvn' command directly
                sh 'mvn clean test'
            }
        }
    }
}
