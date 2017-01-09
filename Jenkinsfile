
#!groovy
def environment, helloworld,stage0,scm

fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
		environment = fileLoader.load('vars/environment');
		stage0 = fileLoader.load('vars/stage0');
		scm = fileLoader.load('vars/scm');
	
stage ('Preparation') {
	environment.dumpEnvVars()			
	}
}	
stage ('Checkout') {
	node { scm.checkout('https://wwwin-svn-jrsm.cisco.com/nds/ch_repo/tags/vgs3/acman')  }
}
