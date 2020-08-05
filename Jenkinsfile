pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'hello world'
          }
        }

        stage('Building') {
          steps {
            echo 'In process'
          }
        }

      }
    }

    stage('testing') {
      steps {
        echo 'Testing...'
      }
    }

    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            echo 'deploying'
          }
        }

        stage('git') {
          steps {
            echo 'git hello'
          }
        }

      }
    }

  }
}