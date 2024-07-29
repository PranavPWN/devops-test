pipeline {
        agent any
        stages {
         
          stage("Build & SonarQube SAST Scanner") {
            agent any
            steps {
              withSonarQubeEnv('Sonarscan') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
