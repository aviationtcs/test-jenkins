node {
  stage('SCM Checkout'){
    git 'https://github.com/aviationtcs/test-jenkins'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven-ec2', type: 'maven'
    sh "${mvnHome}/bin/mvn package"    
  }
}
