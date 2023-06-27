@Library('my-shared-library') _

pipeline{

    agent any
      tools {
    maven "maven3.8.1"
      }

    stages{
        stage('Git Checkout'){    
            steps{
            gitCheckout(
                branch: "main",
                url: "https://github.com/chuks0684/mrdevops_java_app.git"
            )
            }
        } 
       -X switch
        stage('Unit Test maven'){
         steps{
             sh "mvn package"
       }
    }
}
}    
