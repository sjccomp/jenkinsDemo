pipeline {
   agent any
	
   stages {
   	  stage ('Initialize') {
            steps {
                
                    echo "PATH = ${PATH}"
                  	echo "M2_HOME = ${M2_HOME}"
                
            }
        }
   
      stage('Hello') {
         steps {
            sh 'mvn test'
         }
      }
   }
}