#!groovy
def environment, helloworld
stage ('Load Build files from GitHub') {
fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
	helloworld = fileLoader.load('vars/helloworld');
	environment = fileLoader.load('vars/environment');
	scm = fileLoader.load('vars/scm');
	}
}
stage ('Run methods from the loaded content') {
	helloworld.printHello("Good morning!")
	environment.dumpEnvVars()
	node { scm.checkout('https://wwwin-svn-jrsm.cisco.com/nds/ch_repo/tags/vgs3/deviceman/3.0.1-1/')}
}
