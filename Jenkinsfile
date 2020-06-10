pipeline {
     agent any
     stages {
         stage('Upload to AWS') {
            steps {
                withAWS(region:'us-east-2', credentials:'aws-static') {
                    // do something
                    s3Upload(pathStyleAccessEnabled: true, payloadSigningEnabled: true, file:'index.html', bucket:'jenkins-bansari-project-3')
                }
            }
        }
    }
}
