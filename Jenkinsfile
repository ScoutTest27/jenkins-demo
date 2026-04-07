pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning code...'
            }
        }

        stage('Build') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run App') {
            steps {
                sh 'node index.js'
            }
        }
    }
}
