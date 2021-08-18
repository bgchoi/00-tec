pipeline {
  agent any
  stages {
    stage('push-schedule') {
      steps {
        build 'SchedulePushSendMessageChunkJob'
      }
    }

  }
}