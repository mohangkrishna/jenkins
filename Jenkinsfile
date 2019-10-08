node {
 stage ('SCM checkout'){
   git 'https://github.com/mohangkrishna/jenkins'
 }
 stage ('compile'){
  def mvnHome = tool name: 'm3', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
 }
 stage ('Deploy') {
  sh 'ssh root@192.168.0.112 mkdir -p /var/www/temp_deploy'
  sh 'scp -r /var/lib/jenkins/workspace/sai/target root@192.168.0.112:/var/www/temp_deploy/'
}
}
 
