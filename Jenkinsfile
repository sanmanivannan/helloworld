pipeline {
  agent any
  stages {
    stage('Validate') {
      steps {
        sh 'echo "validate step"'
        git(url: 'git \'https://github.com/sanmanivannan/helloworld.git\'', branch: 'master')
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