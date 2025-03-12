/*node {
	
	//  Declarative syntax
		echo "Build"
    	echo "test"
		echo "Integration test"
	
	/*scripted syntax
	stage('Build') {
		echo "Build"
	}
	stage('Test') {
		echo "Test"
	}
	stage('Integration Test'){
		echo "integartion testing"
	}
}*/
pipeline{
	//agent any 
	agent { docker{image 'maven:3.6.3'}}
	stages{
		stage('build'){
			steps{
				sh 'mvn --version'
				echo "build"
			}
		}
		stage('test'){
			steps{
				echo "test"
			}
		}
		stage('deploy'){
			steps{
				echo "deploy"
			}
		}
	}
	post{
		always{
			echo " i have run successfully"
		}
		success{
			echo "great work yuvraj"
		}
		failure{
			echo "you failed"
		}
	}
}