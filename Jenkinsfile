pipeline {
  agent any
  stages {
    stage('Validate') {
      steps {
        git(url: 'git \'https://github.com/sanmanivannan/helloworld.git\'', branch: 'master')
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
