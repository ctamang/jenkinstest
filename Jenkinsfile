pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                bat "mvn clean jenkinstest/MyApp/pom.xml"
            }
        }
        stage('Test') {
            steps {
                bat "mvn test jenkinstest/MyApp/pom.xml"
            }
        }
        stage('Deploy') {
            steps {
                bat "mvn package jenkinstest/MyApp/pom.xml"
            }
        }
    }
 }
