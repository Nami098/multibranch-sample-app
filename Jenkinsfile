pipeline {
  agent any
  options {
    buildDiscarder(logRotator(numToKeepStr: '1'))
  }
  stages {
    stage('Build') {
      steps {
        //sh '''
        
        echo 'testing webhooks'
        echo 'build multibranch pipeline here.'
        
        //'''
      }
    }
  }
  post {
    always {
        junit(
          allowEmptyResults: true, 
          testResults: '**/build/test-results/test/*.xml'
        )
    }
  }
}
