pipeline {
  agent {
    node {
      label "172.31.38.55"
    }
  }
  stages {
    stage ("slave-1") {
      steps {
      // sh "sudo yum install httpd -y"
        sh "sudo cp -r /home/ec2-user/workspace/deploy-gitcode-to-slave/Vel-Assignment/index.html /var/www/html/"
               sh "sudo service httpd restart"
      }
    }
     }
      }
