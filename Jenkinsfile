pipeline {
  agent {
    node {
      label 'node-label'
    }

  }
  stages {
    stage('print hello world') {
      agent {
        node {
          label 'fakeLabel'
        }

      }
      steps {
        echo 'Hello World'
      }
    }

    stage('print node version') {
      steps {
        sh 'node -v'
      }
    }

  }
}