pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                script {
                    // Récupération du code source depuis la branche
                    checkout scm
                }
            }
        }

        stage('Build') {
            steps {
                script {
                    // Étapes de construction (compilation avec Maven)
                    sh 'mvn clean install'
                }
            }
        }

        // ... autres étapes du pipeline ...

    }

    post {
        always {
            // Actions à effectuer toujours après l'exécution du pipeline
        }
    }
}
