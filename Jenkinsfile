pipeline {
    agent any

   stages {
         stage('init') {
            steps {
                sh 'terraform init'
            }
        }
         stage('validate') {
            steps {
                sh 'terraform validate'
          }
        }
         stage('plan') {
            steps {
                sh 'terraform plan'
         }
       }
         stage('apply') {
            steps {
                sh 'terraform apply --auto-approve'
        }
      }
        stage('destroy') {
            steps {
                sh 'terraform destroy --auto-approve'
        }
      }
}
}
