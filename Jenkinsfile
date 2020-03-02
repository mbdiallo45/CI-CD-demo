 
 #!groovy
 pipeline{
    agent any
    stage('CheckoutModule1') {
        steps {
            sh 'mkdir -p Module1'
            dir("Module1")
            {
                git branch: "master",
                credentialsId: '074f3bfa-9aac-4a0b-be69-e2aa21f418dd',
                url: 'https://github.com/mbdiallo45/maven-exemple.git'
            }
        }
   }

 }
 
 
   
