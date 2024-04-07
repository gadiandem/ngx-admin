pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/gadiandem/ngx-admin.git'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'ng build --prod'
            }
        }
//         stage('Deploy') {
//             steps {
//                 // Add deployment steps here, e.g., using AWS CLI or S3 plugin
//             }
//         }
    }
}
