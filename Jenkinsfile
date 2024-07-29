pipeline {
        agent none
        stages {
         
          stage("Build & SonarQube SAST Scanner") {
            agent any
            steps {
              withSonarQubeEnv('Sonar') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
