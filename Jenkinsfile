pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/ibrahim180101/Car-Details-website.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo cp -r * /var/www/html/
                sudo systemctl restart apache2
                '''
            }
        }
    }
}
