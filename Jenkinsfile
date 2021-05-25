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
    stage('build and test app')
    {
      steps{
        sh 'node app.js'
      }
    }
  }
}
