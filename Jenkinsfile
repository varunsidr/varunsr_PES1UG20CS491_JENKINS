pipeline{
  agent any
  stages{
    stage('Build'){
    steps{
    sh 'g++ -c PES1UG20CS491.cpp'
    sh 'g++ -o PES1UG20CS491 PES1UG20CS491.cpp'
    echo 'Build  Success'
   }
  }
  stage('Test'){
    steps{
      sh './PES1UG20CS491'
      echo 'Test Success'
     }
    }
    stage('eploy'){
    steps{
    echo 'Deployment Success'
    }
   }
  }
  post{
    failure{
    echo 'Pipeline Failed'
   }
  }
 }
  
