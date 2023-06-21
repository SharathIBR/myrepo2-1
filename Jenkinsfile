pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          agent any
          steps {
            sh 'echo "Step1"'
            sh 'echo "Step2"'
            sh 'echo "Step3"'
          }
        }

        stage('Stage2') {
          agent any
          steps {
            echo 'Step4'
            echo 'Step5'
          }
        }

      }
    }

    stage('Stage3') {
      agent any
      steps {
        sh 'echo "This is in Stage 3 Step1"'
      }
    }

  }
}