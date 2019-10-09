pipeline {
  agent any
  stages {
    stage('Pull') {
      steps {
        git(url: 'https://github.com/Somesh16/Narendraapplication.git', branch: 'master')
      }
    }
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            bat 'mvn build'
          }
        }
        stage('Maven') {
          steps {
            bat 'mvn build'
          }
        }
      }
    }
  }
}