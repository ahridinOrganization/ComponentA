#!groovy
def environment

fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
	environment = fileLoader.load('vars/environment'); 
}	
	
stage ('Preparation') {
	environment.dumpEnvVars()			
}
