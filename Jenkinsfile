pipeline {
        agent any
        stages {
         
          stage("Build & SonarQube SAST Scanner") {
            agent any
            steps {
              withSonarQubeEnv('SonarQube Scanner') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
