pipeline {
    agent any
    tools {
        maven 'Maven3'  // Jenkins -> Global Tool Config -> Maven
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
//New branch to push into central repo
//new comment to test auto trigger using the webhook
//new commnet to test webhook again
