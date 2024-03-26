@Library('shared_library') _ 

pipeline{
    agent any
    parameters{
        choice(name: 'action', choices: 'create\ndelete', description: 'Choose create/Destroy')
    }
    stages{
        when {expression {
            params.action == 'create'
        }}
        stage('Checkout Code'){
            steps{
                script{
                    gitCheckout("https://github.com/vikash-kumar01/mrdevops_java_app.git", "main")
                    
                }
            }
        }
        //stage('Unit test'){
           // steps{
             //   script{

             //       unitTest()
               // }
           // }
       // }
       // stage('Integration test'){
           // steps{
               // script{
                    
                   // integrationTest()
                // }
           // }
        // }
        stage('Static Code Analysis'){
            steps{
                script{
                    
                    staticCodeAnalysis()
                }
            }
        }
    }
}