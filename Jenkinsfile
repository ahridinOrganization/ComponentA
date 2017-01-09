#!groovy
def environment, helloworld
stage ('Preparation') {
	fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
		helloworld = fileLoader.load('vars/helloworld');
		environment = fileLoader.load('vars/environment');
		scm = fileLoader.load('vars/scm');
	helloworld.printHello("Good morning!")
	environment.dumpEnvVars()			
	}
}	
stage ('Checkout') {
	node { scm.checkout()}
}
