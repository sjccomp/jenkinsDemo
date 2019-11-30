pipeline{
 	agent any
 	
 	stages{
 		stage('testing stage'){
 		  steps{
 		    withMaven(maven){
 		      sh 'mvn test'
 		    }
 		  }
 		}
 	}
}