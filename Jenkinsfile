@Library('my-shared-library') _

pipeline{

    agent any

    stages{
        stage('Git Checkout'){    
            steps{
            gitCheckout(
                branch: "main",
                url: "https://github.com/chuks0684/mrdevops_java_app.git"
            )
            }
        }
        stage('Unit Test maven'){
        steps{
               script{
                   
                   mvnTest()
               }
        }
    }
}
}    
