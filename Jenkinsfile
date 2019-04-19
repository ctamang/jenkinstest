pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                bat "mvn clean -f MyApp/pom.xml"
            }
        }
        stage('Test') {
            steps {
                bat "mvn test -f MyApp/pom.xml"
            }
        }
        stage('Deploy') {
            steps {
                bat "mvn package -f MyApp/pom.xml"
            }
        }
    }
 }
