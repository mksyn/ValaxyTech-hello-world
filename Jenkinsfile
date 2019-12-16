pipeline {
    agent any 
    stages {
        stage('SCM Checkout') { 
            steps {
                git 'https://github.com/mksyn/ValaxyTech-hello-world.git' 
            }
        }
  
        stage('Maven Build') { 
            steps {
                sh label: '', script: 'mvn clean install' 
            }
        }  
        stage('Junit') { 
            steps {
                sh label: '', script: 'mvn test' 
            }
        }         
    }  
}  
