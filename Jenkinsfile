def mvnhome
node {
stage ('Build') {
if (isUnix()) {
mvnhome = tool 'maven'
sh "'${mvnhome}/bin/mvn' -Dmaven.test.failure.ignore clean install"
} else {
mvnhome = tool 'maven'
bat(/"${mvnhome}\bin\mvn" -Dmaven.test.failure.ignore clean install/)
}
}
}
