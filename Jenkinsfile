pipeline {
    agent any
 
    stages {
        stage('Test') {
            steps {
                bat "mvn -D clean test"
            }
    }
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
}      
}
