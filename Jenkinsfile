pipeline {
    agent any 
    tools {
    maven 'M3'
  }
    stages {
        stage('----  clean -----') { 
            steps {
               
               sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package" 
            }
        }
    }
}
