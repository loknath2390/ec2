node{
  stage('SCM checkout'){
    git 'https://github.com/loknath2390/ec2.git'
   }
   stage('Compile-Package'){
    sh 'mvn package'   
   }
}
