pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                // Clean workspace before cloning
                deleteDir()

                // Clone the repository
                git 'https://github.com/shripadrithe/demo.git'
            }
        }
    }
}
