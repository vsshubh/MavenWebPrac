pipeline {
    agent any

    tools {
        maven 'MAVEN'
        jdk 'JDK'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/vsshubh/MavenWebPrac.git'
            }
        }

        stage('Build WAR') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
