@Library('my-shared-library') _

pipeline{

    agent any
    tools{
     maven 'maven3.8.1'

      }
    stages{
         
        stage('Git Checkout'){
            steps{
            gitCheckout(
                branch: "main",
                url: "https://github.com/cloudtechnoli/javaproject1.git"
            )
            }
	}
	stage('Unit test maven'){
	  steps{
	    script{
	      mvnTest()
	          }
	      }

        }
     } 
}
