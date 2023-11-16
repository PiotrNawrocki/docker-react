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
                docker run -e CI=true piotrnawrocki/docker-react npm run test
            }
        }
    }
}