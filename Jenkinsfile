#!/usr/bin/env groovy

pipeline {
  agent {
        docker {
            image 'node'
        }
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building NPM...'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }
    }
}
