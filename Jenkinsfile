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
    
      steps {
      
        script {
          echo 'Stage 2'
          whoami
          sh label: '', script: './runJava.sh'
        
          }
        }
    }
  }
}
