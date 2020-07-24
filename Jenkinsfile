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
 
  stage('Slack Notification'){
    slackSend baseUrl: 'https://hooks.slack.com/services/', 
      channel: 'test_jenkins_1', color: 'good', 
      message: 'Welcome to slack Jenkins Notifications', 
      teamDomain: 'test-sn44454', 
      tokenCredentialId: 'Slack_Demo', 
      username: 'gopinath.m@prodapt.com'
  }

  
  
}
