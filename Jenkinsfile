pipeline {
  agent any
    stages {
  stage('Clone sources') {
      steps {
        script {
          echo 'Stage 1'
          git 'https://github.com/bencygeo/Test_Jenkin.git'
          name "Ben"
          echo "hello $(name)"
        }
      }
    }
  stage('Stage build') {
    
      steps {
      
        script {
          echo 'Stage 2'
          
          sh label: '', script: 'bash ./runJava.sh'
        
          }
        }
    }
     
  }

}
