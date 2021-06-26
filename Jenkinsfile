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
        echo 'deploy completed'
      }
    }

  }
}