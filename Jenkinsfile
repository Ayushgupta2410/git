pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Ayushgupta2410/calculator.git'
            }
        }

        stage('Build') {
            steps {
                bat 'javac src\\*.java'
                bat 'jar cfm CalculatorApp.jar manifest.txt -C src .'
            }
        }
    }
}

