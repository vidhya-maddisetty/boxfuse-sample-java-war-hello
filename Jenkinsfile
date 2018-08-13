node {
stage ('Build') {
if (isUnix()) {
sh "/usr/bin/mvn -Dmaven.test.failure.ignore clean install"
} else {
bat(/"/usr/bin/mvn" -Dmaven.test.failure.ignore clean install/)
} 
}
}
