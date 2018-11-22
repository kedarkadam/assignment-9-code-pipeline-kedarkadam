Pipeline {
 agent { label 'linux' }
 stages {
  stage ('Unit Tests') {
    Steps {
    sh 'ant -f test.xml -v'
    junit 'reports/results.xml'
    }
  stage ('Build') {
    Steps {
    Sh ant -f build.xml -v
    }
  }
}
