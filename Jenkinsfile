// Declarative pipeline
pipeline {
    agent any
    
    stages {
       stage('Git Checkout Stage') {
           steps {
               git credentialsId: 'a71391eb-198c-413c-9b96-2608f6f34351', url: 'https://github.com/vijayalaxmiduvva/newproject.git'
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
