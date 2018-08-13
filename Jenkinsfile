node {
def mvnhome
echo "github clone"
stage ('gitclone') {
git 'https://github.com/vidhya-maddisetty/boxfuse-sample-java-war-hello.git
}
stage ('Build') {
if (isUnix()) {
sh "'/usr/bin/mvn' -Dmaven.test.failure.ignore clean install"
} else {
bat(/"${mvnhome}\bin\mvn" -Dmaven.test.failure.ignore clean install/)
}
 
}

}
