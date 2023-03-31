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
            stage('INTEGRATION TESTING') { 
              
               steps {
                
                script{ 
                     sh 'mvn verify -DskipunitTests'
                    }
                  
                }
            }
            stage('Maven Build') { 
              
               steps {
                
                script{ 
                     sh 'mvn clean install'
                    }
                  
                }
            }



        }
    }