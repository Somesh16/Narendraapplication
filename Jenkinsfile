pipeline {
  agent any
  stages {
    stage('Pull') {
      steps {
        git(url: 'https://github.com/Somesh16/Narendraapplication.git', branch: 'master')
      }
    }
    stage('Build') {
      steps {
        bat 'mvn compile'
      }
    }
  }
}