pipeline {

agent { node { label 'master' } }
tools {
        maven 'maven 3.6.3'
        jdk 'jdk1.8'
    }
stages {
        stage('Code validate') {
            steps {
                sh 'mvn validate'
            }
        }
       stage('Code Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Code Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Code package') {
            steps {
                sh 'mvn package'
            }
        } 
    
    
    }
}