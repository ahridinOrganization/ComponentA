//@Library('github.com/cloudbeers/multibranch-demo-lib') _
fileLoader.withGit('github.com/cloudbeers/multibranch-demo-lib', 'master', null, '')
def standardBuild = fileLoader.load('vars/standardBuild');

standardBuild {
    environment = 'golang:1.5.0'
    mainScript = '''
go version
go build -v hello-world.go
'''
    postScript = '''
ls -l
./hello-world
'''
}
