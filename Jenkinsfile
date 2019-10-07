node {
 stage ('SCM checkout'){
   git 'https://github.com/mohangkrishna/jenkins/tree/master'
 }
 stage ('compile'){
   sh 'mvn clean install'
 }
}
 
