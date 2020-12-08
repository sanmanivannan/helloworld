pipeline {
  agent any
  stages {
    stage('Validate') {
      steps {
        sh 'echo "validate step"'
      }
    }

    stage('Compile') {
      steps {
        sh 'echo "compile step"'
      }
    }

    stage('package') {
      steps {
        build 'package'
      }
    }

  }
}