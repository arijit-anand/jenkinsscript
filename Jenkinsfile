pipeline{
  agent any
  
  stages{
    stage("print"){
      steps{
        echo "Hello World arijit anand"
      }
    }
    stage("current build"){
      steps{
        echo "The current build is ${currentBuild.number}"
      }
    }
  }
}
