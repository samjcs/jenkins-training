pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Run WS Scan') {
            steps {
                bat 'java -jar "C:\\wss\\wss-unified-agent.jar" -c ".\\wss-unified-agent.config" -d "."' -product jenkinsTraining -project testScan_1
            }
        }
    }
}
