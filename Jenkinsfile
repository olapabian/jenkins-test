pipeline {
    agent any // Używa Javy zainstalowanej bezpośrednio w Twoim systemie/WSL
    stages {
        stage('Checkout') {
            steps {
                checkout scm // Pobiera kod z repozytorium
            }
        }
        stage('Build & Run Java') {
            steps {
                // Kompilujemy i uruchamiamy bezpośrednio poleceniami shell
                sh 'javac Hello.java'
                sh 'java Hello'
            }
        }
    }
}
