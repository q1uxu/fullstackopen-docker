pipeline {
  agent {
    node {
      label '14-alpine'
    }

  }
  stages {
    stage('') {
      steps {
        git(url: 'git@github.com:q1uxu/fullstackopen-docker.git', branch: 'main', changelog: true)
      }
    }

  }
}