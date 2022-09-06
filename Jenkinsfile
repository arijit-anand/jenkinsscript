pipeline{
 agent any
  stages{
    stage("Build"){
      steps{
       echo "${env.BUILD_ID}"
       echo "${currentBuild.number}"
      }
    }
    
    stage("Test"){
      steps{
       bat 'make check || true' 
       junit '**/target/*.xml'
      }
    }
  }
}
