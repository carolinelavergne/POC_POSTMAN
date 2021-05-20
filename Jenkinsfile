pipeline {
    agent any
    stages {
      stage("Npm package installation") {
        steps {
          bat 'npm install'
        }
      }
      stage("Run newman") {
        steps {
          bat 'newman run Newman.json -e Prod.json -d iterationData.csv'
        }
      }
    }
}
        
        
