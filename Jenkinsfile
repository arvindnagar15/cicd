pipeline{
	agent any
	
	stages{
	
		stage('Compile stage'){
			
			steps{
				
				withMaven(maven: 'maven_3.6.1'){
					sh 'mvn clean compile'
				}
			
			}
		
		}
		
		stage('Testing stage'){
			
			steps{
				withMaven(maven: 'maven_3.6.1'){
					sh 'mvn test'
				}
			}
		}
		stage('Deployment stage'){
			
			steps{
				
				withMaven(maven: 'maven_3.6.1'){
					sh 'mvn deploy'
				}
			}
		}
	}
}