pipeline {

  agent any
//    node { label 'workstation' }


  environment {
    NEWRELIC_API_KEY = credentials('ansible1')
    SAMPLE_URL = "google.com"
  }

  stages {

    stage('Foo') {
      steps {
        echo 'Hello world'
        echo 'Bye'
      }
    }

    stage('Bar') {
      steps {
        echo 'Hello world'
      }
    }

  }

  post {
    always {
      echo 'I will always say Hello again!'
    }
  }

}