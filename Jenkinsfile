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
              sh 'cd Frontend'
              sh 'docker build -t insurance:latest .'
          }
    }
    stage('Docker Run'){
          steps{
              echo'Docker building stage'
              sh 'docker run -td -p 8000:8000 insurance:latest '
          }
    }
  }
}
