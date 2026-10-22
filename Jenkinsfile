pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'Plan for development'
      }
    }

    stage('Code') {
      steps {
        echo 'Develop the code'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build the code'
          }
        }

        stage('Test') {
          steps {
            echo 'Test the code'
          }
        }

        stage('Stage') {
          steps {
            echo 'Stage the code'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deploy the code'
          }
        }

        stage('Operate') {
          steps {
            echo 'Operate the code'
          }
        }

      }
    }

  }
}