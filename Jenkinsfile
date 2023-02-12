pipeline {
agent any
stages {
  stage ('clean'){
        steps {
            sh 'mvn clean'
               }
           }
  stage ('validate'){
         steps {
             sh 'mvn validate'
                }
          }
  stage ('Test'){
         steps {
               sh 'mvn test -DskipTests'
               }
           }
    stage ('Package'){
           steps {
               sh 'mvn package -DskipTests'
                 }
           }
           stage ('Verfiy'){
           steps {
               sh 'mvn verify -DskipTests'
                 }
           }
  
  stage ('Install'){
           steps {
               sh 'mvn install -DskipTests'
                 }
           }
}
}
