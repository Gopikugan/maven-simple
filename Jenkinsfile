node{
  
  stage('SCM Checkout'){
    git 'https://github.com/Gopikugan/maven-simple'
  }
  
  
  stage('Compile-Package'){
    bat 'mvn package'
  }
  
  stage('Email Notification'){
    mail bcc: '', body: 'Test_Jenkins_Email_Notification', cc: '', 
      from: 'gopinath.m@prodapt.com', replyTo: '', 
      subject: 'Test_Jenkins_Email_Notification', 
      to: 'gopinath.m@prodapt.com'
  }
}
