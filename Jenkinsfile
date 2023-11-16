pipeline {
    agent { 
        dockerfile {
            filename 'Dockerfile.dev'
            label 'piotrnawrocki/docker-react'
        }
     }
    stages {
        stage("test") {
            steps {
                docker run piotrnawrocki/docker-react npm run test -- --coverage
            }
        }
    }
}