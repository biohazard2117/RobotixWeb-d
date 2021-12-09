pipeline {
  agent any
  stages {
    stage('Down') {
      steps {
        echo 'Shutting down all the containers'
        sh '''docker-compose down
docker ps '''
      }
    }

    stage('Up') {
      steps {
        echo 'Refreshing and starting all the containers now'
        sh '''docker-compose up -d --no-recreate
docker ps'''
      }
    }

    stage('') {
      steps {
        echo 'All containers are up and running'
      }
    }

  }
}