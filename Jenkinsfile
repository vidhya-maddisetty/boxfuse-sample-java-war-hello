node {
 tools {
    maven 'maven'
  }
stage ('gitclone') {
git 'https://github.com/vidhya-maddisetty/boxfuse-sample-java-war-hello.git
}
stage ('Build') {
if (isUnix()) {
sh "mvn -Dmaven.test.failure.ignore clean install"
} else {
bat(/"mvn" -Dmaven.test.failure.ignore clean install/)
} 
}
}
