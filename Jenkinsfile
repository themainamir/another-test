pipeline {

  agent any
  parameters {
      choice(name: 'CHOICES', choices: ['1.1.1', '2.2.2', '3.3.3'], description: 'choose your version')
  }
  
  stages {
      stage('‌Build') {
          steps {
              echo 'this is building stage..'
              echo "Your favorite fruit is ${params.CHOICES}"
          }
      }
      stage('Test') {
        when {
          expression {
              params.CHOICES == '1.1.1'
          }
        }
          steps {
              echo 'this is testing 1.1.1'
          }
      }
      stage('Deploy') {
          steps {
              echo 'this is deploying stage..'

          }
      }
  }
}
