pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Récupérer le code source depuis le référentiel Git
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Compiler le projet avec Maven
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Exécuter des tests unitaires
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // Déployer l'application
                // (Remplacez par les commandes de déploiement spécifiques à votre projet)
            }
        }
    }
}
