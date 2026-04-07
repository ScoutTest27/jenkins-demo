pipeline {
    agent any

    stages {
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

        stage('Deploy') {
            steps {
                sh 'docker build -t demo-app .'
                sh 'docker run -d -p 3000:3000 demo-app'
            }
        }
    }
}
            }
        }
    }
}
