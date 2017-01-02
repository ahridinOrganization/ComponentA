#!groovy
developer {
  checkoutScm()
  rake 'unittest[--report=build/report.xml]'
  reportJunit 'build/report.xml'  // will publish the test report
  optional { rake 'audit' }  // to mark stages which are not critical
  rake 'uml'
  reportHtml(name: 'UML', path: 'build/html')  // will upload an arbitrary HTML Report
  rake 'test variant=release'
  rake 'deploy prefix=export'
}


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