pipeline {
    agent {
	label {
	label "master"
	customWorkspace "/mnt/multibranch"
	}
	}
    stages {
        stage('main') {
            steps {
                sh "cp -r /mnt/multibranch/jenkins-multibranch/index.html /var/www/html/"
				sh "chmod -R 777 /var/www/html/index.html"
            }
        }
    }
}
