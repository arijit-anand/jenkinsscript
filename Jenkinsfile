pipeline{
  agent any
  stages{
    stage("build"){
    steps{ 
      echo "This is build step"
    }
    }
    
    stage("deploy")
    {
      stages{
        stage("deploy-sequential"){
          steps{
           echo "This is deployment sequential" 
          }
        }
        
        stage("build-sequential")
        {
          steps{
            echo "This is build sequential" 
          }
        }
      }
  }
}
}
