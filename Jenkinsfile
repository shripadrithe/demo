pipeline {
    agent any
    stages {
        stage('Checkout from Git') {
            steps {
                script {
                    // Checkout code from Git repository
                    git branch: 'main', url: 'https://github.com/shripadrithe/demo.git'
                }
 }
 }
    stage('Copy Index HTML') {
          steps {
                script {
                    // Remove existing files in the destination folder
                    sh 'rm -rf /var/www/html/*'
                    // Copy files from Jenkins workspace to destination folder
                    sh 'cp -r "/var/lib/jenkins/workspace/apache-wh_main env"/* /var/www/html/'
                }
            }
        }
    }
}
