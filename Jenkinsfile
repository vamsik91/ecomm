    pipeline {
        agent any 
        stages {
            
            stage('Git Hub code ') { 
            
               steps {
                   git 'https://github.com/vamsik91/ecomm.git'
                }
            }

            stage('Test the app') { 
               steps {
                   sh 'mvn test'
                }
            } 
        }
    }