pipeline {
  agent any
  stages {
    stage('Developement') {
      steps {
        echo 'Dev success'
      }
    }

    stage('Deploy to QA') {
      steps {
        echo 'DeploytoQASuccess'
      }
    }

    stage('SmokeTest') {
      parallel {
        stage('SmokeTest') {
          steps {
            echo 'SmokeSuccess'
          }
        }

        stage('Performance') {
          steps {
            echo 'PerformanceSuccess'
          }
        }

      }
    }

  }
}