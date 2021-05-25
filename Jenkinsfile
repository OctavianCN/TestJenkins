pipeline
{
  agent any
  stages{
    stage('git clone')
    {
      steps{
        sh 'rm -rf TestJenkins'
        sh 'git clone https://github.com/OctavianCN/TestJenkins.git'
      }
    }
    stage('install express')
    {
      steps{
        sh 'npm install express'
      }
    }
    stage('test app')
    {
      steps{
        sh 'rm test.sh'
        sh 'cp /test.sh .'
        sh 'cp /test2.sh .'
        sh 'cat test.sh'
        sh 'cat test2.sh'
        sh './test.sh'
        sh './test2.sh'
      }
    }
  }
}
