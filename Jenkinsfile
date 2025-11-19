pipeline {
    agent { 
        docker { image 'python:3.9-alpine' } 
    }
    stages {
        stage('Vérification Python') { 
            steps { 
                sh 'python --version'
                sh 'echo "Ce script tourne DANS un conteneur Docker !"'
            }
        }
    }
}