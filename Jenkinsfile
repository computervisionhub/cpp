pipeline{
  	agent any
	stages{	
		stage('Build'){
			steps{
				sh 'echo "building.."'
				sh 'pwd'
				sh 'ls'
				sh 'cd jenkins_calculator'
				sh 'ls'
				sh 'bash cmake_build.sh'
			}
		}
	}
}
