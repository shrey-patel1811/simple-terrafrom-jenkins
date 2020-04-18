#!/usr/bin/env groovy
//Above line is for Shebang

def credentialsId = 'awsCredentials'

node {
   stage('Checkout') {
       echo 'Hello from Stage 1'
       cleanWs()
   }
    stage('init') {
        echo env.AWS_ACCESS_KEY_ID
        echo env.AWS_SECRET_ACCESS_KEY
        sh 'terraform init'
    }
}
