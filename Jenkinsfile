pipeline{
  agent any
  
  environment{
    M2_HOME = "/home/ec2-user/apache-maven-3.6.3"
  }
  stages{
    stage("checkout"){
      steps{
        checkout scm
      }
    }
    
    stage("unit Test"){
      steps{
        sh '${M2_HOME}/bin/mvn clean test:test'
      }
    }
  }
}
