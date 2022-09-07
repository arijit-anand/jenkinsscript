pipeline {
    agent any
    
    environment {
        no="1"
        name="arijit"
    }
    
    stages{
        stage("printenv"){
            steps{
                bat "printenv | sort"   
            }
        }
    }
}
