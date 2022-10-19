node {
  stage('SCM Checkout'){
    git 'https://github.com/aviationtcs/test-jenkins'
  }
  stage('Email Notification') {
    mail bcc: '', body: '''Hi,
    Welcome to learn jenkins
    Thanks''', cc: '', from: '', replyTo: '', subject: 'Jenkins job status', to: 'fav.songs9891@gmail.com'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven-ec2', type: 'maven'
    sh "${mvnHome}/bin/mvn package"    
  }
}
