pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''apt install curl -y
curl -o- -L https://yarnpkg.com/install.sh | bash
yarn install'''
      }
    }

  }
}