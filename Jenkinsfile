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
				sh 'chmod +x cmake_build.sh'
				sh 'bash cmake_build.sh'
				archiveArtifacts artifacts: 'jenkins_calculator/build/calculator', fingerprint: true
			}
		}
		stage('Test'){
			steps{
				sh 'echo "testing.."'
				sh './jenkins_calculator/build/calculator'
			}
		}
	}
}
