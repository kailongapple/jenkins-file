pipeline {
  agent any
  stages {
    stage('clone') {
      steps {
        git(changelog: true, poll: true, url: 'https://github.com/kailongapple/jenkins-file', branch: '"${release}-${UUID.randomUUID().toString()}"')
      }
    }

  }
  environment {
    worddir = '/opt/nginx/html'
  }
}