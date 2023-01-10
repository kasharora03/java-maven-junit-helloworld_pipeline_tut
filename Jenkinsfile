pipeline {
    agent {
        label 'docker-maven-slave'
    }
    
    tools {
        maven 'maven-mixin'
    }

    stages {
 /*   stage('Source Control Mgnt') {
            steps {
                git branch: 'main', credentialsId: '54d6a6bc-c70b-44a7-9db6-fcb5d9f66131', url: 'https://github.optum.com/kbisen1/java-maven-junit-helloworld.git'
            }
        } */
        
            stage('Source Control Mgnt') {
            steps {
                git branch: 'main', credentialsId: '1ee7a4e6-f0c1-489f-96ae-283cec5a9250', url: 'https://github.optum.com/kbisen1/java-maven-junit-helloworld.git'
            }
        } 


    
    stage('Build the JAR') {
            steps {
                sh label: '', script: 'mvn clean package install'
            }
        }
        
    }
}
