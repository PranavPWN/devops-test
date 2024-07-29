node {
  stage('SAST') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def scannerHome = tool 'Sonarscan';
    withSonarQubeEnv() {
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}
