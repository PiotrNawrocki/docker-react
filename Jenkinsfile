pipeline {
    agent { 
        dockerfile {
            filename 'Dockerfile.dev'
        }
     }
    stages {
        stage("test") {
            steps {
                sh 'npm run test -- --coverage'
            }
        }
    }
}