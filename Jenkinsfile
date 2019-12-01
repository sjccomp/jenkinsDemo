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
                //bat 'mvn test' 
                bat "mvn clean verify"
                //junit 'build/surefire-reports/*.xml'
            }
            post {
                success {
                    echo "hello world" 
                }
            }
        }
    }
}
