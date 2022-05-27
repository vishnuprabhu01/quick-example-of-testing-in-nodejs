
pipeline {
  agent {label 'Node_npm'}
    
  stages {
        
    stage('source code') {
      steps {
        git branch: 'master', url: 'https://github.com/vishnuprabhu01/quick-example-of-testing-in-nodejs.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
             }
    } 
    stage('test') {
        steps {
            sh 'npm run start'
                    }
    }
  } 
}
