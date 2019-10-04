pipeline {
  agent any
  stages {
  stage('Clone sources') {
      steps {
        script {
          echo 'Stage 1'
          git 'https://github.com/bencygeo/Test_Jenkin.git'
          
        }
      }
    }
  stage('Stage build') {
    withEnv(['PATH+EXTRA=/usr/sbin:/usr/bin:/sbin:/bin']){
      steps {
        script {
          echo 'Stage 2'
          sh label: '', script: 'runJava.sh'
        }
      }
    }
    }
  }
}
