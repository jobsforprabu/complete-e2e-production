pipeline {
    agent any
    tools {
      jdk 'java'
      maven 'my-maven'
    }

    stages {
        stage("cleanup workspace") {
            steps{
                cleanWs()
            }
        }
    }

    stages {
        stage("checkout from scm") {
            steps {
                git branch: 'main', url: 'https://github.com/jobsforprabu/complete-prodcution-e2e-pipeline'
            }
        }
    }
}