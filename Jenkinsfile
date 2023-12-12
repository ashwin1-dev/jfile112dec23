pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
            sh 'sudo rm -rf /var/www/html'
            sh 'sudo yum install httpd -y'
            sh 'sudo systemctl start httpd'
            sh 'sudo git clone https://github.com/ashwin1-dev/web-farm.git  /var/www/html'
            }
        }
    }
}
