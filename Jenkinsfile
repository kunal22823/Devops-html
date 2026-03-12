pipeline{
  agent any
  stages{
    stage('Checkout'){
      steps{
        git 'https://github.com/kunal22823/Devops-html.git'
      }
    }
    stage('Publish'){
      steps{
        publishHTML([
          allowMissing:true,
          alwaysLinkToLastBuild:false,
          keepAll:false,
          reportDir:'.',
          reportFiles:'index.html',
          reportName:'My Html pipeline'
        ])
      }
    }
  }
}
