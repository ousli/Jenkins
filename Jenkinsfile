pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Étape de compilation"'
                sh 'ls -lah'               // Affiche le contenu du dossier
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Étape de tests"'
                // Ici mets tes vraies commandes de test, exemple :
                // sh 'python -m unittest'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Étape de déploiement"'
                // Mets ici ta commande de déploiement (simulée ou réelle)
            }
        }
    }
}
