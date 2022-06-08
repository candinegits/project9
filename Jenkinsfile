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
	stage('build x'){
		steps{
	sh'action build x'
	}
	}
	stage('build y'){
		steps{
			sh'action build y'
		}
	}
	stage('build c'){
		steps{
			sh'action build c'
		}
	}
	}
	}
}
