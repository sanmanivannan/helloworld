pipeline {
  agent any
  stages {
    stage('Validate') {
      steps {
        sh 'echo "validate step"'
      }
    }

    stage('Unit Test') {
      parallel {
        stage('Unit Test') {
          steps {
            sh 'echo "compile step"'
          }
        }

        stage('Integrtaion Test') {
          steps {
            sh 'echo "Integration Step"'
          }
        }

        stage('Performance Test') {
          steps {
            sh 'echo "Performance Test"'
          }
        }

      }
    }

    stage('package') {
      steps {
        sh 'echo "package done"'
      }
    }

    stage('Deploy') {
      when {
        branch 'master'
      }
      steps {
        sh 'echo "Deploy to Prod"'
      }
    }

  }
}