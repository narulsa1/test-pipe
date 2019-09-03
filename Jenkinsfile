pipeline {
    agent any
      stages {
          stage ('Build') {
              steps {
                  sh 'echo "Hello World!!! This is my first pipe" > /var/www/html/index.html'
              }
          }
          stage ('Test') {
              steps {
                  sh 'curl -I http://192.168.1.56'
              }
          }
      }
      post {
          success {
              echo 'This stage is successful.'
          }
      }
}
