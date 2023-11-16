pipeline {
    agent { 
        dockerfile {
            true
            filename 'Dockerfile.dev'
        }
     }
    stages {
        stage("test") {
            steps {
                sh 'docker run piotrnawrocki/docker-react npm run test -- --coverage'
            }
        }
    }
}