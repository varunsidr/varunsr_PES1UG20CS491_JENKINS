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
      sh './PES1UG20CS490'
      echo 'Test Success'
     }
    }
    stage('Deploy'){
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
  
