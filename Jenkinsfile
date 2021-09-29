node {
  stage('SCM') {
    git 'https://github.com/kolizox55/jenkins-sonar.git'
  }
  stage('SonarQube analysis') {
    def scannerHome = tool 'test-demo';
    withSonarQubeEnv('demo') { // If you have configured more than one global server connection, you can specify its name
      bat "D:\sonar-scanner-4.6.2.2472-windows\bin"
    }
  }
}
