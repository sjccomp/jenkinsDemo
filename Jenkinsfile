pipeline {
    agent any
    
    stages {
        stage ('Initialize') {
            steps {
               echo "PATH = ${PATH}"
                echo "M2_HOME = ${M2_HOME}"
               
            }
        }

        stage ('Build') {
            steps {
                bat 'mvn test' 
            }
            post {
                success {
                    echo "hello world" 
                }
            }
        }
    }
}