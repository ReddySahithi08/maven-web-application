node
{
 def mavenHome = tool name: "maven3.8.6"
 stage('CheckoutCode')
 {
  git branch: 'development', credentialsId: '597b1247-0ba5-4c35-8d0d-6834b29b5ef7', url: 'https://github.com/ReddySahithi08/maven-web-application.git'
 }
 stage('Build')
 {
  sh "${mavenHome}/bin/mvn clean package"
 }
  /*
 stage('ExecuteSonarQubeReport')
 {
  sh "${mavenHome}/bin/mvn sonar:sonar"
 }
 stage('UploadArtifactIntoNexus')
 {
  sh "${mavenHome}/bin/mvn deploy"
 }
 stage('DeployApplicationIntoTomcat')
 {
  sshagent(['0f672cc7-7106-41f5-a3b1-8cc3b602f790'])
  {
   sh "scp -o  StrictHostKeyChecking=no target/maven-web-application.war ec2-user@65.2.152.216:/opt/apache-tomcat-9.0.65/webapps"
  }
 }
 stage('SendEmailNotification')
 {
 mail bcc: '', body: '''Build Over...

 regards,
 sahithi''', cc: 'surapusahithi9@gmail.com', from: '', replyTo: '', subject: 'Build Over', to: 'surapusahithi@gmail.com'
 }
 */
}
