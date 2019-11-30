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
         steps(maven : "Maven 3.6.3") {
            sh 'mvn test'
         }
      }
   }
}