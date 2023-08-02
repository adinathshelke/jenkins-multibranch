pipeline {
    agent {
	label {
	label "master"
	customWorkspace "/mnt/multibranch"
	}
	}
    stages {
	    stage ('git clone') {
		    steps {
	    sh "git clone https://github.com/adinathshelke/jenkins-multibranch.git -b 23Q2"
		    }
		    }
        stage('main') {
            steps {
                sh "cp -r /mnt/multibranch/jenkins-multibranch/index.html /var/www/html/"
				sh "chmod -R 777 /var/www/html/index.html"
            }
        }
    }
}
