node{
  stage('SCM checkout'){
    git 'https://github.com/loknath2390/ec2.git'
   }
   stage('Compile-Package'){
     def mvnHome = tool name: '', type: 'maven'
     sh "${mvnHome}/bin/mvn package"
   }
}
