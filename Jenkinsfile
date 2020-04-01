// Declarative pipeline
pipeline {
    agent any
    
    stages {
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
