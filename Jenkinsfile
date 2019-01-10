node {
stage ('Build') {
checkout scm
sh "/usr/bin/mvn -Dmaven.test.failure.ignore clean install"
}
stage ('Archieve Artifacts') {
archiveArtifacts artifacts: '*.war', onlyIfSuccessful: true
}
 stage ('Display Artifact') {
 sh "ls -ltr *.zip"  
 }   
 }
