pipeline {
  agent any

  stages {
    stage('Terraform Init') {
      steps {
        script {
          sh 'terraform init'
        }
      }
    }

    stage('Terraform Plan') {
      steps {
        script {
          sh 'terraform plan'
        }
      }
    }

    stage('Terraform Apply') {
      steps {
        script {
          sh 'terraform apply -auto-approve'
        }
      }
    }
  }
}
