pipeline{
     
    tools{
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
       }
      
     agent any
        stages{
            stage('clone repo'){
           
            steps{
                
		 git credentialsId: '97e0bf41-61ee-4e7c-b23a-8fe60c8a3d0b', url: 'https://github.com/anil-5619/jenkins1.git'   
                }
				}
             stage('Compile'){
                
                  
                steps{
                    git credentialsId: 'mygit', url: 'https://github.com/ashisnishanka/realtimecodeNEW.git'
                    sh 'mvn compile'
                }
                
            }
		//multi anil
            stage('CodeReview'){
               steps{
                    echo "code review is succesfully"
                }
                
            }
            stage('UnitTest'){
			
                steps{
                    echo "code review is succesfully"
					sh 'mvn test'
                
                }
                
            }
            stage('MetriCheck'){
               steps{
                    echo "code review is succesfully"
                } 
                
            }
            stage('Package'){
                
               steps{
                    echo "code review is succesfully"
					sh 'mvn package'
                } 
            }
		stage(' QA deploy'){
              steps{
                    echo "code review is succesfully"
                }  
            }
			
		stage(' dev deploy'){
                
              steps{
                    echo "code review is succesfully"
                } 
            }
            
        }
    
    }
