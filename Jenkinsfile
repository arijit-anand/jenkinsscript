pipeline {
    agent any
    
    environment {
        no="1"
        name="arijit"
    }
    
    stages{
        stage("printenv"){
            steps{
                echo "The value of no is ${env.no}, The type is ${env.no.class}"
                echo "The value of name is ${env.name}, The type is ${env.name.class}"
            }
        }
    }
}
