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
                sh "rm -rf *"
                sh "yum install httpd -y"
                sh "git clone https://github.com/anilbichkule/Vel-Assignment.git -b master"
                sh "cp -r /mnt/git/Vel-Assignment/index.html /var/www/html/"
               sh "service httpd restart"
            }
    }
  }
}
