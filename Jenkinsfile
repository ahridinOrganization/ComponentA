#!groovy
def environment

fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
	stage0 = fileLoader.load('vars/stage0'); 
}	
	
stage ('Preparation') {
	stage0.printHello("STAGE-0")			
}
