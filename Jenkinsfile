pipeline {
    agent any
    stages {
        steps('Upload to AWS') {
            withAWS(region:'us-west-2', credentials: 'Static HTML publisher in AWS'){
                s3Upload(file: 'index.html', bucket: 'jenkins-devops-class', path: 'index.html')
            }
        }
    }
}