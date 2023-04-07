pipeline {

  agent any
  parameters {
      choice(name: 'CHOICES', choices: ['1.1.1', '2.2.2', '3.3.3'], descreption: 'choose your version')
  }
  
  stages {
      stage('‌Build') {
          steps {
              echo 'this is building stage..'
              echo "Your favorite fruit is ${params.CHOICES}"
          }
      }
      stage('Test') {
          steps {
              echo 'this is testing stage..'
          }
      }
      stage('Deploy') {
          steps {
              echo 'this is deploying stage..'

          }
      }
  }
}
