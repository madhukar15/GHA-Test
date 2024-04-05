pipeline {
    agent none

    stages {
        stage('Deploy on Server 1') {
            agent {
                label 'server1'
            }
            steps {
                script {
                    // Execute Docker Compose commands or scripts to start your application on server 1
                    echo "hello"
                    sh 'docker-compose up -d'
                }
            }
        }
        stage('Deploy on Server 2') {
            agent {
                label 'server2'
            }
            steps {
                script {
                    // Execute Docker Compose commands or scripts to start your application on server 2
                    sh 'docker-compose up -d'
                }
            }
        }
    }
}
