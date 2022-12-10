pipeline {
    agent any

    stages {
        
        stage('clone the project') {
            
            steps {
                 git "https://github.com/fadysaoudy/addressbook"
            }
        }
        
        stage('compile') {
            
            steps {
                sh "mvn compile"
            }
        }
        
        stage('tests') {
            
            steps {
                sh "mvn test"
            }
        }
       
        stage('pakage') {
            
            steps {
                sh "mvn package"
            }
        }
    }
}
