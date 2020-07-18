pipeline{
  	agent any
	stages{	
		stage('Build'){
			steps{
				sh 'echo "building.."'
				sh 'pwd'
				sh 'ls'
				sh 'cd jenkins_calculator'
				sh 'bash build.sh'
			}
		}
	}
}
