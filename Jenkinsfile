pipeline {
 agent any
 stages {
 stage('build') {
 steps {
sh 'echo "I am in build step"'
sh 'sh test.sh'
 }
 }
 }
post {
 success {
 archiveArtifacts artifacts: 'test.sh', fingerprint:
true
 }
 }
}
