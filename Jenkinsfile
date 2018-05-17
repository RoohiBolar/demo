pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'cat README.md && hello world'
      }
    }
    stage('cleanup') {
      steps {
        cleanWs(cleanWhenAborted: true, cleanWhenFailure: true, cleanWhenNotBuilt: true)
      }
    }
  }
}