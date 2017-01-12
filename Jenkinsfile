@Library('github.com/ahridinOrganization/jenkinsDSL') _

generate_job_stage0 {
    jobName='deviceman_stage_0'
    repoUrl='https://wwwin-svn-jrsm.cisco.com/nds/ch_repo/trunk/vgs3/deviceman'
    tagUrl='https://wwwin-svn-jrsm.cisco.com/nds/ch_repo/tags/vgs3/acman'
    //checkoutMode='CheckoutUpdater'
    jdkVersion='1.7'
    mavenVersion='Maven 3.0.4'
    mavenGoals='clean install pmd:pmd findbugs:findbugs clover2:instrument clover2:clover'
    mavenPom='pom.xml'
    slaveLabel='vgs'
    timeout=120
    mailNotification="kuku@cisco.com"
}

build job: "deviceman_stage_0"
