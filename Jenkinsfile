pipeline{
 agent any
  stages{
    stage("Build"){
      steps{
       echo "${env.BUILD_ID}"
       echo "${currentBuild.number}"
      }
    }
  }
}
