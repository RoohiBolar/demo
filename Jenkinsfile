pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh ''' cat README.md && echo hello world
'''
      }
    }
    stage('cleanup') {
      steps {
        cleanWs(cleanWhenAborted: true, cleanWhenFailure: true, cleanWhenNotBuilt: true)
      }
    }
    stage('slack') {
      steps {
        echo 'slack'
      }
    }
  }
}