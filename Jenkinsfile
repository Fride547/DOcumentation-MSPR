pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'whoami'
            }
        }
        stage('Test') {
            steps {
                sh 'ls -l'
                sh 'rm -rf /var/www/html/*'
                sh 'cp * /var/www/html'
                sh 'ls -l /var/www/html'
            }
        }
        
        stage('Run application') {
            steps {
                sh 'java -jar go-secure.jar cberthier.html'
                
            }
        }
    }
}

