pipeline {
   agent any
   stages {
      stage ('Compile') {
        steps {
           withMaven(maven : 'apache-maven-3.6.1') {
           bat'mvn clean compile'
              }
          }
         }
     stage ('Testing') {
       steps {
           withMaven(maven : 'apache-maven-3.6.1') {
           bat'mvn test'
             }
         }
        }
    stage ('Deploy') {
      steps {
          withMaven(maven : 'apache-maven-3.6.1') {
          bat'mvn install'
            }
         }
        }
     }
   }
