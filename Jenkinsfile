#!groovy
def environment, helloworld

fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
		helloworld = fileLoader.load('vars/helloworld');
		
	
stage ('Preparation') {
	helloworld.printHello("Good morning!")	
	}
}	
