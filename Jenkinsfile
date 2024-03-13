pipelineJob('MyPipelineJob') {
  definition {
    cpsScm {
      scm {
        git {
          remote {
            url('https://github.com/umairshah124/Seed_Jobs.git')
          }
          branch('*/main')
        }
      }
      lightweight()
    }
  }
}
