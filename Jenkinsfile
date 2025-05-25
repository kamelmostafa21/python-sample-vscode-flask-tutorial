pipeline{
    agent{
        label "agent-1"
    }
    
    stages{
        stage("build Docker image"){
            steps{
                sh "docker build -t kamelmostafa/python-ci-cd:v${BUILD_NUMBER} ."
            }
        }
        stage("Push Docker image"){
            steps{
                sh "docker push kamelmostafa/python-ci-cd:v${BUILD_NUMBER}"
            }
        }
    }
}