pipelineJob('test-pipeline') {
  definition {
    cpsScm {
      scm {
        git {
          remote {
            credentials('umairshah124')    
            url("https://github.com/umairshah124/Seed_Jobs.git")
          }
          branch('*/main')
        }
      }
      stage('Build') {
    devices = ['device1', 'device2', 'device3']
    devices.each { device ->
        def buildResults = build job: 'Build_Daily', wait: true, propagate: false,
                parameters:[string(name: 'Device', defaultValue: device, description: '', trim: true)]
        println "The result of the downstream job is: ${buildResults.result}"
    }
}
      scriptPath('Jenkinsfile') 
      lightweight()
    }
  }
}
