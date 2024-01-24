node{
// demo
   stage('SCM Checkout'){
     git 'https://github.com/Nagadeops/jen-mvn'
   }
   stage('Compile-Package'){
      // Get maven home path
      def mvnHome =  tool name: 'maven-3', type: 'maven'   
      sh "${mvnHome}/bin/mvn package"
   }
 
   stage('Email Notification'){
      mail bcc: '', body: '''Hi Welcome to jenkins email alerts
      Thanks
      Naga''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'nagasang25@gmail.com'
   }
}
