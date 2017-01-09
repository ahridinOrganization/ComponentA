#!groovy
def environment, helloworld
stage ('===> PREPARATIONS: Load Build files from GitHub') {
fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
	helloworld = fileLoader.load('vars/helloworld');
	environment = fileLoader.load('vars/environment');
	scm = fileLoader.load('vars/scm');
	}
}
stage ('===> RUN: execute methods from the loaded content') {
	helloworld.printHello("Good morning!")
	environment.dumpEnvVars()
	node { scm.checkout()}
}
