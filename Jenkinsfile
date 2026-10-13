pipeline{
agent {
    label 'docker'
}
stages{
     stage('Build') {
        steps {
            script{
           sh 'docker build -t my-app:latest -f dockerfile.dev .'
        }
    }
    stage('Test') {
        steps {
            script{
                env.DOCKER.BUILDKIT = 1
           sh 'docker run -e CI=true my-app:latest npm run test'
        }
    }
}

}
}
}