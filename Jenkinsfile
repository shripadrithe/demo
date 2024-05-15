pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                script {
                    // Replace 'https://github.com/username/repository.git' with your repository URL
                    def repositoryUrl = 'https://github.com/shripadrithe/demo.git'
                    
                    // Define the directory where you want to clone the repository
                    def directory = '/var/wwww/html'
                    
                    // Clone the repository
                    git branch: 'master', url: repositoryUrl, destination: directory
                }
            }
        }
    }
}
