pipeline{
 agent any
 environment{
   CC="arijit"
 }
  stages{
    stage("Build"){
      steps{
       echo "${CC}"
       echo "${env.BUILD_ID}"
       echo "${currentBuild.number}"
      }
    }
  }
}
