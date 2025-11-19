pipeline {
    agent any
    stages {
        stage('Build') {
            steps { echo 'Build fait.' }
        }
        stage('Validation') {
            steps {
                // Le pipeline va se mettre en pause ici
                input "On déploie en production ?"
            }
        }
        stage('Deploy') {
            steps { echo 'Déploiement en cours...' }
        }
    }
}