#!groovy

fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
	stage0 = fileLoader.load('vars/stage0'); 
	//pipeline = fileLoader.load('vars/pipeline'); 
}	
def myJob = freeStyleJob('SimpleJob')
myJob.with {
    description 'A Simple Job'
}



//pipeline {
//    name = 'git'
//}

