pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                bat "mvn clean MyApp/pom.xml"
            }
        }
        stage('Test') {
            steps {
                bat "mvn test MyApp/pom.xml"
            }
        }
        stage('Deploy') {
            steps {
                bat "mvn package MyApp/pom.xml"
            }
        }
    }
 }
