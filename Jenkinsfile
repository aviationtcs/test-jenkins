node {
  stage('SCM Checkout'){
    git 'https://github.com/aviationtcs/test-jenkins'
  }
  stage('Compile-Package){
      sh 'mvn package'      
  }
}
