node('agent-1') {
    
    stage('Build Docker image') {
        sh "docker build -t kamelmostafa/python-ci-cd-script:v${env.BUILD_NUMBER} ."
    }

    stage('Push Docker image') {
        sh "docker push kamelmostafa/python-ci-cd-script:v${env.BUILD_NUMBER}"
    }
}
