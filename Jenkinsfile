pipeline {
    agent any
    parameters {
      choice(name: 'VERSION', choices: ['1.1.0', '1.2.0', '1.3.0'], description: '')
      booleanParam(name: 'executeTests', defaultValue: true, description: '')
    }
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
  steps {
      echo 'testing the application...'
  }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                echo "deploying version ${params.VERSION}"
            }
        }
    }
}
