pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh ''' 
                cd vite-project
                npm install
                '''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh ''' 
                cd vite-project
                npm run dev
                '''
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}