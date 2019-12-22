#!groovy
node('slave') {
   // Mark the code checkout 'stage'....
   stage ('Checkout'){
 gradle4=tool 'gradle4'
      // Get some code from a GitHub repository
      checkout scm
      
   }

   // Mark the code build 'stage'....
   stage ('gradle build'){
      { 
      sh $"{gradle4/bin/gradle build"
      }
   } catch (ex) {
      echo 'Error occured'
     stage ('post') {
     if ( CurrentBuild.result == 'SUCCESS')
           addBadge(icon: 'green.gif', text: 'build success')
        
}
}
      
