pipeline{
    agent any
    environment {
        PATH = "/usr/share/maven/bin:$PATH"
    }
    stages {
        stage("Get Code From Repo"){
            steps{
                git credentialsId: 'git_credentials', url: 'https://github.com/Prasdey/TestProject.git'
            }
        }
        stage("build"){
            steps{
                sh "mvn clean package"
            }
        }
        
    }
    
}
