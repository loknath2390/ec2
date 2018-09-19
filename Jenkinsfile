node{
  stage('SCM checkout'){
    git 'https://github.com/loknath2390/ec2.git'
   }
   stage('Compile-Package'){
     def mvnHome = tool name: 'Maven', type: 'maven'
     sh "${mvnHome}/bin/mvn package"
   }
  stage('Deploy in tomcat')
    sshagent(['tomcat']) {
      sh 'scp -o StrictHostKeyChecking=no -l target/*.war tomcat@172.31.6.34:/opt/apache-tomcat-7.0.47/webapps/'
   }
}
