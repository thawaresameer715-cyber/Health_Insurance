pipeline{
  agent any
  triggers{
    githubPush()
  }
  stages{
    stage('Hello'){
          steps{
              echo'hello SameerThaware xxxxxxxxxxxxxxxxx'
          }
    }
    stage('Docker Build'){
          steps{
              echo'Docker building stage'
              //sh 'docker build -t '
          }
    }
  }
}
