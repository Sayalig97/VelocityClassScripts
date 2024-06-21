pipeline {

agent {
			label{
						label 'qa'
			}
}

stages{
			stage ('install-tree'){
								steps{
											sh "sudo yum install tree -y"
								}
			}
			
			stage ('install-soft-on-172.31.45.193'){
			agent {
						label {
									label "172.31.45.193"
						}
			}
								steps {
										sh "sudo yum install httpd -y"
										sh "sudo yum install tree -y"
								}
			}
			
			
}
}
