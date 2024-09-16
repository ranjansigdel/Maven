pipeline 
{
	agent any
	tools
	{
		maven 'MAVEN_HOME'
	}
	
	stages{
		stage('Welcome Master Branch')

		{
			steps
			{
				echo 'Welcome to Jenkins Pipeline'
			}			
		}
		stage('Checkout') 
		{
        		steps 
			{                
           			 git 'https://github.com/hkshitesh/DEVOPS-B25.git'
        		}
		}
		stage('Clean Stage')
		{
			steps
			{
				bat 'mvn clean'
			}			
		}
		stage('Test Stage')
		{
			steps
			{
				bat 'mvn test'
			}			
		}
		stage('Pre-Build Stage')
		{
			steps
			{
				echo 'This is Pre-Build Stage'
			}			
		}
		stage('Build Stage')
		{
			steps
			{
				bat 'mvn install'
			}			
		}
		stage('Post-Build Stage')
		{
			steps
			{
				echo 'This is Post Build Stage'
			}			
		}
		stage('Java Version Check Stage')
		{
			steps
			{
				bat 'java --version'
			}			
		}
		
		stage('Success Stage')
		{
			steps
			{
				echo 'Successfully Build Thanks'
			}			
		}
	
	}
}
