pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'im building'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'im testing'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploying'
          }
        }

      }
    }

  }
}