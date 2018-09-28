@Library('shared-pipeline') _
onePipeline()

stage ('Sonar Analysis') {
      steps {

          withSonarQubeEnv('local-sonarqube') {
              sh "${scannerHome}/bin/sonar-scanner"
          }
      }
  }
