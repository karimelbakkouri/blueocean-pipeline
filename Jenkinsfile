pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build completed'
      }
    }

    stage('Tests ') {
      parallel {
        stage('Test1') {
          steps {
            echo 'run test1'
          }
        }

        stage('test2') {
          steps {
            echo 'run test2'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'are you sure to deploy?', ok: 'yes, i m sure')
        echo 'deploy completed'
      }
    }

    stage('Notify new build') {
      steps {
        echo 'new build done'
      }
    }

  }
}