@Library('my-shared-library') _

pipeline{

    agent any

    stages{
         
        stage('Git Checkout'){
                    when { expression {  params.action == 'create' } }
            steps{
            gitCheckout(
                branch: "main",
                url: "https://github.com/cloudtechnoli/javaproject1.git"
            )
            }
	}
    }
}

