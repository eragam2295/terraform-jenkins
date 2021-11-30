pipeline{
  agent any
  stages{
    stage('terraform init and apply - dev'){
      steps{
	    sh "sh returnstatus: true, script: 'terraform workspace new dev"
		sh "terraform init"
		sh "terraform apply -var-file=dev.tfvars -auto-approve"
		}
    }
	}
