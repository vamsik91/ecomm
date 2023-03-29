pipeline {
    agent any

    stages {
        stage('Git clone the Code') {
            steps {
                script{
                    sh 'git 'https://github.com/vamsik91/ecomm.git''
                }
            }
        }
        stage('Unit Test') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
       }
        stage('Unit Test') {
            steps {
                echo 'Testing..'
            }
        }
    }
}