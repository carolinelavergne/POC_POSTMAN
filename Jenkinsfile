pipeline {
    agent any
    stages {
      stage("Npm package installation") {
        steps {
          bat label: 'install NPM package', script: 'npm install'
        }
      }
      stage("Run newman") {
        steps {
          bat label: 'run newman', script: 'newman run Newman.json -e Prod.json -d iterationData.csv'
        }
      }
    }
}
        
        
