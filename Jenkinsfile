pipeline {
    agent any
    stages {
        stage("build") {
            steps {
                docker
                docker build -t piotrnawrocki/docker-react -f Dockerfile.dev .
            }
        stage("test") {
            steps {
                docker run -e CI=true piotrnawrocki/docker-react npm run test
            }
        }
    }
}