pipeline{
  agent any
  stages{
    stage('Checkout'){
      steps{
        git 'https://github.com/kunal22823/Devops-html'
      }
    }
    stage('Publish'){
      steps{
        publishHTML([
          allowmissing:true,
          alwaysLinktoLastBuild:false,
          keepAll:false,
          reportDir:'.',
          reportFiles:'index.html',
          reportName:'My Html pipeline'
        ])
      }
    }
  }
}
