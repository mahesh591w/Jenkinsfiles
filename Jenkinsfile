pipeline {
		agent {
				label {
						label "built-in"
						customWorkspace "/mnt/project"
						
				}
		}
		stages {
				stage ('clone-index') {
							
							steps {
									sh "rm -rf *"
									sh "sudo git clone https://github.com/mahesh591w/Jenkinsfiles.git"
									sh "sudo chmod -R 777 /var/www/html/"
									sh "sudo cp -r /mnt/project/Jenkinsfile/index.html /var/www/html/"
									sh "sudo systemctl restart httpd"
							}
						
				}
				
						
				
		}
				
	}
