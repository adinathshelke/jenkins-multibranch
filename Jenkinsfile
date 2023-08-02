pipeline {
    agent {
	label {
	label "master"
	customWorkspace "/mnt/multibranch"
	}
	}
    stages {
	stage ("git clone"){
	 steps {
	 sh "git clone https://github.com/adinathshelke/jenkins-multibranch.git"
	 }
	}
        stage('23Q1') {
            steps {
                sh "cp -r /mnt/multibranch/jenkins-multibranch/index.html /var/www/html/"
				sh "chmod -R 777 /var/www/html/index.html"
            }
        }
    }
}
