pipeline {
    agent any
    tools {
        maven 'maven3'
        jdk 'jdk1.8'
    }
  stages {
    stage('GIT Checkout'){
        steps{
            script{
                git branch : "{master}"
                url: 'https://github.com/Vellaisamy86/Bits-DevOps-Assgnmnt'
                gitInfo = checkout scm
            }
        echo 'Checkout Successful'
        }
    }
    stage('Build with Maven'){
        steps{
            // Build using maven
            script{
                mvn clean package
            }
        }
    }
   // And next stages if you want to define further...
 } // End of stages
} // End of pipeline
