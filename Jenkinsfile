pipeline {
  agent {
    docker {
      image 'python:3-alpine'
    }
    
  }
  stages {
    stage('build docs') {
      agent any
      steps {
        sh 'cd docs'
        sh 'pip install pipenv'
        sh 'pipenv install'
        sh 'pipenv run make html'
        archiveArtifacts 'docs/_build/html/*'
      }
    }
  }
}