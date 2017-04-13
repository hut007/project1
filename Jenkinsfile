pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        parallel(
          "Build": {
            echo 'Building'
            sh 'pwd'
            timeout(time: 60) {
              sh 'sleep 3'
              echo 'Slept for 2 seconds'
            }
            
            
          },
          "Build2": {
            echo 'Building Build2'
            
          }
        )
      }
    }
  }
  environment {
    DRINK = 'whey'
    FOOD = 'potato'
  }
}