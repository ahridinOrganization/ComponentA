#!groovy

stage 'Load files from GitHub'
def environment, helloworld
fileLoader.withGit('https://github.com/ahridinOrganization/jenkinsDSL.git', 'master', null, '') {
    helloworld = fileLoader.load('vars/helloworld');
    environment = fileLoader.load('vars/environment');
}
stage 'Run methods from the loaded content'
helloworld.printHello()
environment.dumpEnvVars()

//developer {
  //checkoutScm()
  //rake 'unittest[--report=build/report.xml]'
  //reportJunit 'build/report.xml'  // will publish the test report
  //optional { rake 'audit' }  // to mark stages which are not critical
  //rake 'uml'
  //reportHtml(name: 'UML', path: 'build/html')  // will upload an arbitrary HTML Report
  //rake 'test variant=release'
  //rake 'deploy prefix=export'
//}


//#!groovy
//@Library('github.com/ahridinOrganization/jenkinsDSL') _
//Commands {
//}

//@Library('github.com/cloudbeers/multibranch-demo-lib') _
//standardBuild {
    //environment = 'golang:1.5.0'
    //mainScript = '''
//go version
//go build -v hello-world.go
//'''
  //  postScript = '''
//ls -l
//./hello-world
//'''
//}
