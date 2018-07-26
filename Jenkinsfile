pipeline {
  agent { label '' }
  environment {
    awesomeVersion = sh(returnStdout: true, script: 'echo 0.0.1')
  }
  stages {
    stage('output_version') {
      steps {
        git url: 'https://github.com/rajaramthumati/ansible-pipeline.git'
        sh "ansible-playbook -vvvv test.yml --extra-vars \'{\"stage\":\"$var1\"}\' "
        
      }
    }
  }
}
