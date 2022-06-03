pipeline {
	agent any {

		stages {
			stage('SCM') {
				steps {
					git 'https://github.com/SUNILKUMARKUMAWAT371/practice-jeknins.git'
				}
			}

			stage('Build') {
				steps {
					sh 'sudo yum install httpd -y'
					sh 'sudo systemctl start httpd'
					sh 'sudo echo "Welcome to my EMPIRE" > index.html'
					sh 'sudo cp index.html /var/www/html'
				}	
			}	
		}	
	}	
}	
