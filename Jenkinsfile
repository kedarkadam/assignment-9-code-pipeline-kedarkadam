pipeline 
{
 agent { label 'linux' }
  stages {
      stage ('Trial') {
       steps {
    echo 'Hello'
       }
      }
   stage ('Unit Tests') {
    steps {
    sh 'ant -f test.xml -v'
    junit 'reports/*.xml'
    }
   }
  }
}
