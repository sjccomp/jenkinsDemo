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
                junit 'build/reports/**/*.xml'
            }
            post {
                success {
                    echo "hello world" 
                }
            }
        }
    }
}