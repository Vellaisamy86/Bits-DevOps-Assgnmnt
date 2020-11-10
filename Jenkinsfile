pipeline {
    agent any
  stages {
    stage('GIT Checkout'){
    steps{
        // Clone repo
            git branch: 'master',
            credentialsId: 'github',
            url: 'https://github.com/Vellaisamy86/Bits-DevOps-Assgnmnt'
    }
    }
    stage('Mvn Package'){
    steps{
     // Build using maven
        mvn clean package
    }
    }
   // And next stages if you want to define further...
 } // End of stages
} // End of pipeline
