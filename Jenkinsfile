@Library('shared_library') _ 

pipeline{
    agent any
    stages{
        stage('Checkout Code'){
            steps{
                script{
                    gitCheckout(
                        branch: "main"
                        url: "https://github.com/vikash-kumar01/mrdevops_java_app.git"
                    )
                }
            }
        }
    }
}