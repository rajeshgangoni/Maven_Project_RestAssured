pipeline{
    agent any
    environment {
        PATH = "$PATH:/opt/apache-maven-3.8.6/bin"
    }
    stages{
       stage('GetCode'){
            steps{
                git branch: 'main', url: 'https://github.com/rajeshgangoni/Maven_Project_RestAssured.git'
            }
         }        
       stage('Build'){
            steps{
                sh 'mvn clean package'
            }
         }
    }
}  