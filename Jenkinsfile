pipeline 
{
 agent { label 'linux' }
  stages {
      stage ('Trial') {
       steps {
    echo 'Hello, this is a trial!'
       }
      }
   stage ('Unit Tests') {
    steps {
    sh 'ant -f test.xml -v'
    junit 'reports/result.xml'
    }
   }
   stage ('Build'){
    steps {
    sh 'ant -f build.xml -v'
    }
   }
  }
}
