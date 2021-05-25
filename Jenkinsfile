pipeline
{
  agent any
  stages{
    stage('git clone')
    {
      sh 'rmdir -r TestJenkins'
      sh 'git clone https://github.com/OctavianCN/TestJenkins.git'
    }
    stage('install express')
    {
      sh 'npm install express'
    }
    stage('build app')
    {
      sh 'node app.js'
    }
    stage('test app')
    {
      sh 'curl -i localhost:3000'
    }
  }
}
