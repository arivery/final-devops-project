pipeline {

    agent any

	tools{
		maven "Maven3'
	}
	
    stages {

     stage('Clonerepo') {
        steps {
         git 'https://github.com/arivery/final-devops-project.git/'
        }
     }
     
     stage('Compile') {
        steps {
          sh 'mvn compile'
        }
     }
	 
	 stage('UnitTesting') {
        steps {
          sh 'mvn test'
        }	
	 }
		 stage('Package') {
        steps {
          sh 'mvn package'
        }
      }
	 
     
    }
}
