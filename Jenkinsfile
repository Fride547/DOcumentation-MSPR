pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
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
    }
}

