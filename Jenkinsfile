pipeline {
    agent any
    tools (nodejs 'node')
    stages {
        stage('clone git repo'){
            steps{
                git 'git@github.com:pharesd/gallery.git'
            }
        }
        stage('Install project dependencies') {
            steps {
                echo 'Installing the project dependencies'
                sh 'npm install'
            }
        }
        stage('Build') {
            steps{
                sh 'npm run build'
            }
        }

    }

