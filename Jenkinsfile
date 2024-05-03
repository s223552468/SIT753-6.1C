pipeline {
 agent any
 environment {
 STAGING_SERVER = 'Azure_staging_level.gmail.com'
 PRODUCTION_SERVER = 's223552468.com'
 RECIPIENT_EMAIL = 'Hirdyansh.aus42@gmail.com'
 }
 stages {
 stage('Build') {
 steps {
echo 's223552468'
 echo 'This Pipleline is in building stage'
 sh 'echo "./gradlew clean assemble"'
 }
 }
 stage('Unit and Integration Tests') {
 steps {
echo 's223552468'
 echo 'Running test for unit and integratation by s223552468 '
sh 'echo "Using Spock for unit tests,JMockit for integration tests"'
 }
 post {
 always {
 emailext(
 subject: "Jenkins Build by s223552468 #${BUILD_NUMBER} - Tests: ${currentBuild.currentResult}",
 body: "Please see the attached logs for more details.",
 to: "${RECIPIENT_EMAIL}",
attachLog: true
 )
 }
 }
 }
 stage('Code Analysis') {
 steps {
echo 's223552468'
 echo 'Code Analysis is being performed by s223552468'

 sh 'echo " My Code Analysis tool is  CodeClimate"'
 }
 }
 stage('Security Scan') {
 steps {
echo 's223552468'
 echo ' Security scan is being 
performed by s223552468'
 sh 'echo "The tool used is  Burp Suite"'
 }
 post {
 always {
 emailext(
 subject: "Jenkins Build by s223552468 #${BUILD_NUMBER} -Status: ${currentBuild.currentResult}",
 body: "View   the attached information of pipeline in term of logs  for more details.",
 to: "${RECIPIENT_EMAIL}",
attachLog: true
 )
 }
 }
 }
 stage('Deploy to Staging') {
 steps {
echo 's223552468'
 echo 'This pipleline is being Deployed to staging environment by s223552468'
sh "echo 'Deploying to ${STAGING_SERVER}'"
 }
 }
 stage('Integration Tests on Staging') {
 steps {
echo 's223552468'
 echo 'Running integration tests on staging server'
 sh 'echo "Running integration tests on staging server"'
 }
 }
 stage('Deploy to Production') {
 steps {
echo 's223552468'
 echo 'Now after success S223552468 is Deploying the script to production environment'
 sh "echo 'Deploying to ${PRODUCTION_SERVER}'"
 }
 }
 }
 post {
 failure {
     
 emailext(
 subject: "Jenkins Build by s223552468 #${BUILD_NUMBER} - Failed",
 body: "There was a problem with the build.Check jenkins log to debug the issue.",
 to: "${RECIPIENT_EMAIL}",
 attachLog: true
 )
 }
 }
}
