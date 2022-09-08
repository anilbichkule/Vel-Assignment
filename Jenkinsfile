pipeline {
  agent {
    node {
      label "172.31.38.55"
    }
  }
  stages {
    stage ("slave-1") {
      steps {
        sh "sudo rm -rf *"
      // sh "sudo yum install httpd -y"
        sh "sudo git clone https://github.com/anilbichkule/Vel-Assignment.git -b qa"
        sh "sudo cp -r /home/ec2-user/workspace/multi-pipeline_qa/Vel-Assignment/index.html /var/www/html/"
               sh "sudo service httpd restart"
      }
    }
     }
      }
