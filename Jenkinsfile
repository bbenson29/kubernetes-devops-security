pipeline {
  agent any

  stages {
      stage('Build Artifact') {
            steps {
              sh "mvn clean package -DskipTests=true"
              archive 'target/*.jar' 
            }
        }  
<<<<<<< HEAD
     stage('Unit Tests - JUnit and Jacoco') {
      steps {
        sh "mvn test"
      }
      post {
        always {
          junit 'target/surefire-reports/*.xml'
          jacoco execPattern: 'target/jacoco.exec'
        }
      } 
=======
      stage('unit Test') {
            steps {
              sh "mvn test"
             
            }
        }    
>>>>>>> 1ae7191ee592c921a4d2f88ab06874fa58320e99
    }
}