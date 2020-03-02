 
pipeline{
 agent any
 stages {
  stage('CheckoutModule1') {
        steps {
            sh 'mkdir -p Module1'
            dir("Module1")
            {
             stage ('checkout') {
              steps {
                git branch: "master",
                credentialsId: '074f3bfa-9aac-4a0b-be69-e2aa21f418dd',
                url: 'https://github.com/mbdiallo45/maven-exemple.git'
              }
             }
             stage ('Build'){
              steps {
                sh '/usr/share/maven/bin/mvn clean install -B -U -Dsurefire.useFile=false'
              }
             }  
           }
        }
   }
 }
}
 
 
   
