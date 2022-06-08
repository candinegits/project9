pipeline{
	agent any
	stages{
		stage('version control'){
			steps{
				sh'git checkout'
			}
		}
	stage( 'compile and build'){
	parallel{
	stage('build x'){
	steps
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