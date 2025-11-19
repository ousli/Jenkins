pipeline {
    agent any
    stages {
        stage('Création de fichier') {
            steps {
                // On crée un faux fichier de résultat
                sh 'mkdir -p build'
                sh 'echo "Resultat important" > build/mon-app.txt'
            }
        }
        stage('Test') {
            steps {
                // On simule un test réussi
                echo 'Les tests sont OK'
            }
        }
    }
    post {
        always {
            // On archive le fichier créé pour pouvoir le télécharger
            archiveArtifacts artifacts: 'build/mon-app.txt', fingerprint: true
            echo 'Nettoyage terminé.'
        }
    }
}