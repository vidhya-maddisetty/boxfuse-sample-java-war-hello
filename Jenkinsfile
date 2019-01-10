node {
stage ('Build') {
checkout scm
sh "/usr/bin/mvn -Dmaven.test.failure.ignore clean install"
}
stage ('Archive Artifact') {
archiveArtifacts artifacts: 'target/*.war', onlyIfSuccessful: true
}
 stage ('Display Artifact') {
 sh "ls -ltr target/*.war"  
  }   
}
