#!groovy

def environment, helloworld

stage ('Load files from GitHub') {
fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
	helloworld = fileLoader.load('vars/helloworld');
	environment = fileLoader.load('vars/environment');
	}
}
stage ('Run methods from the loaded content') {
	helloworld.printHello()
	environment.dumpEnvVars()
	}

