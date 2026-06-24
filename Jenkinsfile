pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git branch: 'main',
                url: 'https://github.com/ibrahim180101/Car-Details-website.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                cp -r * /var/www/html/
                '''
            }
        }
    }
}
