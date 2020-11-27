pipeline {
  agent any
  stages {
    stage('checkout') {
      parallel {
        stage('checkout') {
          steps {
            git(url: 'https://github.com/tianhongqi/two.git', branch: 'main', changelog: true)
          }
        }

        stage('checkstyle') {
          steps {
            sh 'echo "aaa"'
          }
        }

      }
    }

    stage('build') {
      steps {
        sh 'echo "aaa"'
      }
    }

  }
}