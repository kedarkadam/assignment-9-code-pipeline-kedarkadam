Pipeline 
{
 agent { label 'linux' }
 stages 
 {
  stage ('Unit Tests') 
  {
    sh 'ant -f test.xml -v'
    junit 'reports/results.xml'
  }
  stage ('Build') 
  {
    sh 'ant -f build.xml -v'
  }
 }
}
