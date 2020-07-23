node{
  
  stage('SCM Checkout'){
    git 'https://github.com/Gopikugan/maven-simple'
  }
  
  
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
