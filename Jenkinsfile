#!groovy

fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
	stage0 = fileLoader.load('vars/stage0'); 
	pipeline = fileLoader.load('vars/pipeline'); 
}	
	
//stage ('Preparation') {
stage0()	

//pipeline {
//    name = 'git'
//}

