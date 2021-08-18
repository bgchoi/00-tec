pipeline {
  agent none
  stages {
    stage('push-schedule') {
      steps {
        build 'SchedulePushSendMessageChunkJob'
      }
    }

    stage('Hello1') {
      parallel {
        stage('Hello1') {
          steps {
            echo 'Hello~~1'
          }
        }

        stage('Hello2') {
          steps {
            echo 'Hello~~2'
          }
        }

        stage('Hello3') {
          steps {
            echo 'Hello~~3'
          }
        }

      }
    }

  }
  environment {
    aa = '10'
  }
}