node {
stage ('Build') {
checkout scm
sh "/usr/bin/mvn -Dmaven.test.failure.ignore clean install"
}
}
