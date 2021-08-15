pipeline {

     agent any 
     stages {
          stage ('Build Application') {
             steps {
                      bat 'mvn clean install'
                   }
                 }
                 stage ('Delopy Application into cloudhub') {
                   stages  {
                        bat "mvn clean package deploy -DmuleDeploy"
                        }
                     }
                 }
      }