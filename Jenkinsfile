pipeline{
	agent any
	tools{
		mvn 'maven'
	}
	stages{
		stage('Checkout'){
			steps{
				git branch:'master', url:'https://github.com/PrarthanaAshwath/1.git'
			}	
		}
		stage('Build'){
			steps{
				sh 'mvn clean package'
			}	
		}
		stage('Test'){
			steps{
				sh 'mvn test'
			}	
		}
		stage('Run Application'){
			steps{
				sh 'java -jar target/1-1.0-SNAPSHOT.jar'
			}	
		}
	}
}

		
