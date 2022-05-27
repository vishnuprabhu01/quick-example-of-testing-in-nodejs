
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
            sh 'npm start'
            sh 'node app --location Newcastle'
            sh 'npm test'
            sh 'npm run cover'
        }
    }
  } 
}
