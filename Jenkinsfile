pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build the Software'
      }
    }
    stage('Test') {
      steps {
        sh 'sleep 5'
        sh 'echo tests completed '
      }
    }
    stage('Publish event') {
      steps {
        script {
          publishEvent simpleEvent('testing completed')
        }

      }
    }
  }
}