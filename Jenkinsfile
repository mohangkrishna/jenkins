node {
 stage ('SCM checkout'){
   git 'https://github.com/mohangkrishna/jenkins'
 }
 stage ('compile'){
   sh 'mvn clean install'
 }
}
 
