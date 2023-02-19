pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh 'g++ -o PES1UG20CS615 PES1UG20CS615.CPP'
        echo 'build stage successful'
      }
    }
    stage('Test'){
      steps{
        sh './PES1UG20CS615'
        echo 'test stage succesful'
      }
    }
    stage('Deploy'){
      steps{
        sh 'echo "Deploying"'
        echo 'deployment successful'
      }
    }
  }
  post{
    failure{
      echo 'pipeline failed'
    }
  }
}
