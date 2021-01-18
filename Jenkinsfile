pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
          bat 'hello world'
          }
        }

        stage('Building') {
          steps {
            bat 'In process'
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
