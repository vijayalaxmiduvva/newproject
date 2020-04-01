// Declarative pipeline
pipeline {
    agent any
    
    stages {
       stage('Git Checkout Stage') {
           steps {
               git creddentialId 'github', 
           }
       }
      
       stage('Compile Stage') {
           steps {
               sh "mvn compile"
           }
       }
           
       stage('Package Stage') {
           steps {
               sh "mvn package"
           }
       }    
       
       stage('Deploy Stage') {
           steps {
               sh "mvn tomcat:undeploy"
           }
       }
    }
}    
