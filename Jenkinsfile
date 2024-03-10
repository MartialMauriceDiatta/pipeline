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
                // Compilation du code Java
                bat 'javac HelloWorld.java'
            }
        }
        stage('Test') {
            steps {
                // Exécution du code Java
                bat 'java HelloWorld'
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
>>>>>>> ce9aea819e4f675d5c957bd13b8a898dd86783b2
