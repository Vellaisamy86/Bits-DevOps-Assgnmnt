


pipeline {
  stages {
    stage('GIT Checkout'){
    // Clone repo
    git branch: 'master',
    credentialsId: 'github',
    url: 'https://github.com/Vellaisamy86/Bits-DevOps-Assgnmnt'
    }
    stage('Mvn Package'){
    // Build using maven
    def mvn = tool (name: 'maven3', type: 'maven') + '/bin/mvn'
    sh "${mvn} clean package deploy"
    }
   }
   // And next stages if you want to define further...
 } // End of stages
} // End of pipeline
