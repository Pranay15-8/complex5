
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Python Version') {
            steps {
                bat '"C:\\Users\\prana\\AppData\\Local\\Programs\\Python\\Python310\\python.exe" --version'
            }
        }

        stage('Syntax Check') {
            steps {
                bat '"C:\\Users\\prana\\AppData\\Local\\Programs\\Python\\Python310\\python.exe" -m py_compile app.py'
            }
        }

        stage('Run Application') {
            steps {
                bat '"C:\\Users\\prana\\AppData\\Local\\Programs\\Python\\Python310\\python.exe" app.py'
            }
        }
    }
}
