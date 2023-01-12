pipeline {
  agent any
    stages {
      stage('Semgrep-Scan') {
        steps {
          sh 'pip3 install semgrep'
          sh 'pwd'
          sh 'semgrep --config p/ci --config p/security-audit --config p/secrets'
          //sh 'semgrep --config p/ci --config p/security-audit --config p/secrets --output scan_results.json --json'
      }
    }
  }
}
