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
									sh "sudo git clone https://github.com/mahesh591w/repo1.git"
									sh "sudo chmod -R 777 /var/www/html/"
									sh "sudo cp -r /mnt/project/repo1/index.html /var/www/html/"
									sh "sudo systemctl restart httpd"
							}
						
				}
				
						
				
		}
				
	}
