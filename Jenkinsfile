pipeline{
  agent any
	
  environment{
  	variable="arijit" 
	CRED=credentials("thisisit")
  }
	
  stages{
    stage("build"){
    steps{ 
      echo "This is build step $variable"
      echo '$CRED_USR'
      echo '$CRED_PSW'
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
