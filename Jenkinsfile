#!groovy
def environment, helloworld

fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
		helloworld = fileLoader.load('vars/helloworld');
		environment = fileLoader.load('vars/environment');
		scm = fileLoader.load('vars/scm');
	
stage ('Preparation') {
	helloworld.printHello("Good morning!")
	environment.dumpEnvVars()			
	}
}	
stage ('Checkout') {
	node { scm.checkout('https://wwwin-svn-jrsm.cisco.com/nds/ch_repo/tags/vgs3/acman')}
}
