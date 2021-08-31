pipeline {
    agent any

    stages {
        stage('Build')
        {
            steps 
            {
                echo 'Build application'
            }
        }
        stage('Test')
        {
            steps 
            {
                echo 'test application'
            }
        }
        stage('Deploy')
        {
            steps 
            {
                echo 'deploy application'
            }
        }
    }
    post{
        always
        {
            emailext body: 'summary', subject: 'pipeline status', to: 'amitnankita@gmail.com'
        }
    }
}
