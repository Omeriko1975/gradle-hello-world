#!groovy
node('slave') {
   // Mark the code checkout 'stage'....
   stage ('Checkout'){

      // Get some code from a GitHub repository
      checkout scm
      
   }

   // Mark the code build 'stage'....
   stage ('gradle build'){
      // Get the gradle tool.
      // ** NOTE: This 'maven3' maven tool must be configured
      // **       in the global configuration.
     def gradleHome = tool 'gradle4'

   post  {
   addBadge icon: 'info', id: '', link: '', text: ''
   }
}
