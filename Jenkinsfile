node {
stage ('Build') {
checkout scm
sh "/usr/bin/mvn -Dmaven.test.failure.ignore clean install"
}
stage ('Archive Artifacts') {
archiveArtifacts artifacts: 'target/*.war', onlyIfSuccessful: true
}
 stage ('Display Artifact') {
 sh "ls -ltr target/*.war"  
  }   
}
