pipeline{
  agent any
  stages{
    stage('Maven build'){
      steps{
        echo "this is Jenkinsfile, Demo"
      }
    }
    stage('Dev Deploy'){
      when{
        branch"develop"
      }
      steps{
        echo "Deploying to dev"
      }
    }
    stage('Test Deploy'){
       when{
        branch"test"
      }
      steps{
        echo "Deploying to test"
      }
    }
    stage('Prod Deploy'){
       when{
        branch"main"
      }
      steps{
        echo "Deploying to prod"
      }
    }
  }
}
