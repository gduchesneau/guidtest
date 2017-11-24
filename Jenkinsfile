pipeline {
  agent any
  stages {
    stage('commit') {
      steps {
        retry(count: 3) {
          sleep 4
          sh 'echo \'hello world\''
        }
        
      }
    }
    stage('acceptance') {
      steps {
        sh 'echo \'acceptance\''
      }
    }
  }
}