node{
  stage('SCM checkout'){
    git 'https://github.com/loknath2390/ec2'
   }
   stage('Compile-Package'){
    sh 'mvn compose package'   
   }
}
