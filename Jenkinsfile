pipeline{
	agent any
	stages{
		stage('version control'){
			steps{
				checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/candinegits/project9.git']]])
			}
		}
	stage('compile and build'){
	parallel{
	stage('2-dish usage'){
		steps{
	sh'du -h'
	}
	}
	stage('memory usage'){
		steps{
			sh'free -g'
		}
	}
	stage('cpu check'){
		steps{
			sh'lscpu'
		}
	}
	}
	}
}
}
