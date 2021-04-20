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
        git(url: 'https://github.com/pravinkumarm/ACMEBuild', branch: 'master', poll: true)
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy success'
      }
    }

  }
}