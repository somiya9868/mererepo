pipeline {
 agent any
 stage ('compile stage') {
  steps {
   withMaven(maven: 'maven-4.0.0') {
    sh 'mvn clean compile'
   }
  }
 }
 stage ('testing stage') {
  steps {
   withMaven(maven : 'maven-4.0.0') {
    sh 'mvn test'
  }
  }
 }
 stage ('Deploying stage'){
  steps {
   withMaven(maven: 'maven-4.0.0') {
    sh 'mvn deploy'
 }
 }
 }
}
