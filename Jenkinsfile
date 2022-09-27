pipeline {
  agent {
    node {
      label "172.31.36.194"
    }
  }
  stages {
    stage ("slave-1") {
      steps {
        sh "sudo rm -rf *"
        sh "sudo yum install httpd -y"
        sh "sudo git clone https://github.com/anilbichkule/Vel-Assignment.git -b dev"
        sh "sudo cp -r /home/ec2-user/workspace/multi-pipeline_dev/Vel-Assignment/index.html /var/www/html/"
               sh "sudo service httpd restart"
      }
    }
     }
      }
