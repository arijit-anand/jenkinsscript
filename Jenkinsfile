pipeline{
  agent any
	
  environment{
  	variable="arijit"  
  }
	
  stages{
    stage("build"){
    steps{ 
      echo "This is build step $variable"
    }
    }
    
    stage("deploy")
    {
      parallel{
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
	
	post{
		changed{
			echo "This is your captain speaking!"
		}
	}
}
