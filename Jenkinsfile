pipeline {
    agent any
    stages {
        stage('Pull code') {
            steps {
                sh 'git clone https://github.com/yoda96/node-jenkins-app-example'
                echo ' Code successfully cloned'
            }
        }
        stage('Build stage') {
            steps {

                sh 'npm install --save express'
                sh 'npm install'
                sh 'npm test'
            }
        }
    }
}
