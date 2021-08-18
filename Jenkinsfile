pipeline {
  agent any
  triggers {
        cron('H/5 * * * *')
  }
  stages {
    stage('extract-bbs') {
      steps {
        build 'SgroupBbsExtractBatchJob'
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

    stage('push-schedule') {
      steps {
        build 'SchedulePushSendMessageChunkJob'
      }
    }

  }
}
