pipeline {
    agent any
    stages {
       
        stage('copy all files to html folders') {
            steps {
                sh 'ls -l'
                sh 'rm -rf /var/www/html/*'
                sh 'cp * /var/www/html'
                sh 'ls -l /var/www/html'
            }
        }
        
        stage('Run application') {
            steps {
                sh 'java -jar go-secure.jar sconnor.html'
                
            }
        }

         
    }
}

