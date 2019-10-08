node (label: 'slave') {
 stage ('SCM checkout'){
   git 'https://github.com/mohangkrishna/jenkins'
 }
 stage ('compile'){
  def mvnHome = tool name: 'm3', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
 }
}
 
