pipeline {
    agent any
    
    tools {
        
        maven 'Maven_01'
            }
            
        stages{
                stage('cloning_repo') {
                    steps{
                        git 'https://github.com/gagan889/MavenBuild-Docker-GitHubActions.git'}
                    
                }
                
                stage('compile') {
                    steps{
                        
                        sh 'mvn compile'
                        
                    }
                    
                }
                
                stage('test'){
                    
                    steps{
                        
                        sh 'mvn test'
                        
                    }
                 
                    
                }
                
                stage('Package'){
                    steps{
                        
                        sh 'mvn package'
                        
                    }
                    
                    
                }
             
                }
    
}
