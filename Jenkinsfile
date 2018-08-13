node {
stage ('gitclone') {
git 'https://github.com/vidhya-maddisetty/boxfuse-sample-java-war-hello.git'
}
stage ('Build') {
sh "/usr/bin/mvn -Dmaven.test.failure.ignore clean install"
}
}
