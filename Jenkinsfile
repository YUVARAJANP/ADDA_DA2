pipeline
{
  agent any

  stages {
    stage('Build') {
      steps {
        echo 'Build App'
      }
    }
    stage('Test') {
      steps {
        echo 'Test App'
      }
    }
    stage('deploy') {
      steps {
        echo 'Deploy App'
      }
    }
    post
    {
      failure
      {
        emailext body: 'Summary', subject: 'Pipeline Status', to: 'yuvarajanp71102@gmail.com'

  }
}
