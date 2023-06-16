pipeline {
    agent any
    
    tools{
        jdk 'jdk11'
        maven 'maven_3.0'
    }

    stages {
        stage('GIT CHECKOUT') {
            steps {
                git branch: 'Feature-1', url: 'https://github.com/santhoshsnk/Petclinic.git'
            }
        }
       
        stage('Compile') {
            steps {
                sh  "mvn clean compile"
            }
        }
        stage('Build') {
            steps {
                sh  "mvn clean package -DskipTests=true"
      
        
            }
        }
    }
} 
    
