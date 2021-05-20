pipeline {
    agent any
    
    stages {
      stage("Npm package installation") {
        steps {
          sh 'npm install'
        }
      }
      stage("Run newman") {
        steps {
          sh 'newman run Newman.json -e Prod.json -d iterationData.csv'
        }
      }
    }
}
        
        
