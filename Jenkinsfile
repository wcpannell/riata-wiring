pipeline {
  agent {
    docker {
      image 'python:3-alpine'
    }
    
  }
  stages {
    stage('build docs') {
      steps {
        sh '''cd docs
pip install pipenv
pipenv install
pipenv shell
make html'''
        archiveArtifacts 'docs/_build/html/*'
      }
    }
  }
}