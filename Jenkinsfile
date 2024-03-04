pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Récupérer le code source depuis le dépôt Git
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Compiler le code
                sh 'javac Main.java'
            }
        }
        stage('Test') {
            steps {
                // Exécuter les tests unitaires
                sh 'java -cp .:junit.jar:hamcrest.jar org.junit.runner.JUnitCore MainTest'
            }
        }
        stage('Deploy') {
            steps {
                // Déployer le code sur le serveur de production
                echo "Déploiement sur le serveur de production en cours"
            }
        }
    }
}
