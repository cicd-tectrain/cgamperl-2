pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }

    stage('Deploy') {
        when {
            branch 'feature/*'
            beforeAgent true
        }

      steps {
        echo 'Deploying'
      }
    }

  }
}