pipeline 
{
 agent { label 'linux' }
  stages {
      stage ('Trial') {
    echo 'Hello'
   }
   stage ('Unit Tests') {
    sh 'ant -f test.xml -v'
    junit 'reports/*.xml'
   }
  }
}
