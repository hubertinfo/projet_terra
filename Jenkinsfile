pipeline {
    agent any
    environment {
      GOOGLE_PROJECT_ID = "tf-projet"
      GOOGLE_PROJECT_NAME = "tf-projet"
      GOOGLE_APPLICATION_CREDENTIALS = credentials('terraformkey')
    }
    option {
      skipStagesAfterUnstable()
    }
    stages {
      stage('git'){
        git branch: 'main', credentialsId: '920dca8c-86d6-40e2-b8e4-ea7070df8ee4', url: 'https://github.com/hubertinfo/projet_terra.git'
        }
        stage('terraform init') {
          sh 'terraform init'
        }
        stage('terraform plan') {
          //
        }
        stage('terraform apply') {
          //
        }
    }
}
