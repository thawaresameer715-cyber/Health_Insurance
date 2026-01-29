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
             dir('Frontend'){
                  sh 'docker build -t insurance:a1 .' 
             }
          }
    }
    stage('Docker Run'){
          steps{
              echo'Docker building stage'
              sh 'docker run -td -p 3000:3000 insurance:latest '
          }
    }
  }
}
