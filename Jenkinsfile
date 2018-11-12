pipeline {
   agent any
    tools {
        maven 'mvn'
        jdk 'java 8u192'
         }
   stages   {
      stage ('Preparation') { // for display purposes
      // Get some code from a GitHub repository
         steps {
            sh 'ls -rlt'
         }
      // Get the Maven tool.
      // ** NOTE: This 'M3' Maven tool must be configured
      // **       in the global configuration.           

   }
   stage('Build') {
      // Run the maven build
      steps {
         sh " mvn -Dmaven.test.failure.ignore -Dversion=version clean package"
      } 
   }
  }
}
