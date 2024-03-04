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
                // Compiler le code avec Maven
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                // Exécuter les tests unitaires sur main.java
                sh 'javac -cp .:/path/to/your/junit.jar MainTest.java'
                sh 'java -cp .:/path/to/your/junit.jar:/path/to/your/hamcrest.jar org.junit.runner.JUnitCore MainTest'
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
