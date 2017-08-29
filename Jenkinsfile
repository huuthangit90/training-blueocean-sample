pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        parallel(
          "Hello": {
            sh 'echo Hello World!'
            archiveArtifacts 'test'
            
          },
          "Test-1": {
            sh 'echo Test 1'
            
          },
          "Test-2": {
            sh 'echo Test 2'
            
          }
        )
      }
    }
  }
}