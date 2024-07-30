pipeline {
  agent any
    stages {
      stage('Semgrep-Scan') {
        steps {
          sh 'sudo docker run -e SEMGREP_APP_TOKEN=d53484911e5241c5dd757e5251821baf64e0440e1c29ef56c49a5d12f25fe357 --rm -v "${PWD}:/src" semgrep/semgrep semgrep ci'
      }
    }
  }
}
