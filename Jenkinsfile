pipeline {
    agent {
        node {
            label "built-in"
            customWorkspace "/mnt/git/"
        }
    }
    stages {
        stage ('index-on-master') {
            steps {
                sh "cp -r /mnt/git/Vel-Assignment/index.html /var/www/html/"
               sh "service httpd restart"
            }
    }
  }
}
