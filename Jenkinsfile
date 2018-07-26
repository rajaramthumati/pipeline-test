pipeline {
  agent { label '' }
  environment {
    awesomeVersion = sh(returnStdout: true, script: 'echo 0.0.1')
  }
  stages {
    stage('output_version') {
      steps {
        echo "awesomeVersion: ${awesomeVersion}"
      }
    }
  }
}
