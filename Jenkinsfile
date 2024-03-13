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
      scriptPath('Jenkinsfile') 
      lightweight()
    }
  }
}
