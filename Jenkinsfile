pipeline {
    agent any
    
    environment {
        no="1"
        name="arijit"
        trigger=false
        aws_password=credentials('170ed271-2ec0-42d7-9eb7-309035b4a385')
    }
    
    stages{
        stage("printenv"){
            steps{
                echo "The value of no is ${env.no}, The type is ${env.no.class}"
                echo "The value of name is ${env.name}, The type is ${env.name.class}"
                echo "The value of credentials are ${aws_password}"
            }
        }
        
        stage("something"){
            when{
                expression{
                    trigger.toBoolean()==true   
                }
            }
            
            steps{
                echo "OK"   
            }
        }
    }
}
