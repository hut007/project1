pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
        sh 'pwd'
        timeout(time: 60) {
          sh 'sleep 3'
          echo 'Slept for 2 seconds'
        }
        
      }
    }
  }
  environment {
    DRINK = 'whey'
    FOOD = 'potato'
  }
}