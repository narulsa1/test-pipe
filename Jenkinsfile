pipeline {
    agent any
      stages {
          stage ('build') {
              steps {
                  sh 'echo "Hello World!!! This is my first pipe" > /var/www/html/index.html'
                                }
              }
          stage ('Test') {
              steps {
                  sh 'curl -I http://192.168.1.56'
      }
          }
    post {
            sucess {
              echo 'This stage is successful.'
            }
    }

}
