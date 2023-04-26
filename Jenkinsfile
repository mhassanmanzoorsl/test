pipeline {
    agent any
    
    stages {
        stage('Image Pull') {
            steps {
                withDockerRegistry(credentialsId: 'docker_local_registry', url: 'https://localregistry.com:5000/v2/') {
                sh 'docker push localregistry.com:5000/springbootjacoco:0.0.1'
                }
            }
        } 

    }
}
