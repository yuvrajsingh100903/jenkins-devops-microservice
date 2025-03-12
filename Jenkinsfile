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
	agent any 
	stages{
		stage('build'){
			steps{
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
}