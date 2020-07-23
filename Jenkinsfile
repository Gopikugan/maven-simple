node{
  
  stage('SCM Checkout'){
    git 'https://github.com/Gopikugan/maven-simple'
  }
  
  
  stage('Compile-Package'){
    def mvnHome = tool name: 'Maven 3.6.3', type: 'maven'
    bat "${mvnHome}/bin/mvn package"
  }
}
