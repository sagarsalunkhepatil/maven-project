pipeline {
    agent any


    stages 
    {  
        
        stage ('SCM Checkout') 
	    {
		    steps {	    
          git branch: 'master', url: 'https://github.com/sagarsalunkhepatil/maven-project.git'
         }
    
    }
                              
        stage ('validate') {


            steps {
		withMaven(jdk: 'localjdk-1.8', maven: 'localmaven')     
                              {
                    sh 'mvn validate'
                }
                  }
                                 
        }
		}
		}
		
