node {
 stage('SCM') {
 git 'https://github.com/Josue-lab/MEANStackApp.git'
 }
 stage('SonarQube analysis') {
 // requires SonarQube Scanner 2.8+
 def scannerHome = tool 'sonar-scanner';
 withSonarQubeEnv('My SonarQube Server') {
 sh "${scannerHome}/bin/sonar-scanner"
 }
 }
}
