pipeline {
	agent any
	stages {
	stage ('running build and test parallely')
	parallel {
	stage ('build stage'){ 
	steps sh 'echo "this is build stage"'
	stage ('test stage'){
	steps sh 'echo "this is test stage"'
	}
	}
	}
	}
	stages {
	stage ('deploy stage')
	steps sh 'echo "this is deploy stage"'
	}
	stages {
	stage ('development stage')
	steps sh 'echo "this is development stage"'
	}
}
