pipeline {
  agent any
  environment {
    PATH = "D:/DevTools/apache-maven-3.9.4/bin$PATH"
  }
  stages {
    stage('Git Repo Check') {
      steps {
        checkout scm
      }
    }
    stage('Clone Proj') {
      steps {
        checkout scm
      }       
    }
  }
}
