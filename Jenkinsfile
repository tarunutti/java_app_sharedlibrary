@Library('shared_library') _ 

pipeline{
    agent any
    stages{
        stage('Checkout Code'){
            steps{
                script{
                    gitCheckout("https://github.com/vikash-kumar01/mrdevops_java_app.git", "main")
                    
                }
            }
        }
        stage('Unit test'){
            steps{
                script{

                    unitTest()
                }
            }
        }
        stage('Integration test'){
            steps{
                script{
                    
                    integrationTest()
                }
            }
        }
    }
}