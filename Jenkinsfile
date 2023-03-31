    pipeline {
        agent any 
        stages {
            
            stage('Git Hub code ') { 
            
               steps {
                   git 'https://github.com/vamsik91/JavaWebCalculator.git'
                }
            }

            stage('Test the app') { 
              
               steps {
                
                script{ 
                     sh 'mvn test'
                    }
                  
                }
            } 
        }
    }