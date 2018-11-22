pipeline 
{
 agent { label 'linux' }
  stages {
   stage ('Unit Tests') {
    sh 'ant -f test.xml -v'
    junit 'reports/*.xml'
   }
  }
}
