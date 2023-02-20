pipeline {
    agent any
 
    stages {
        stage('Test') {
            steps {
                bat "mvn -D clean test"
            }
    }
        stage('Deploy') {
            steps {
                bat "mvn -D clean test"
            }
    }
}      
}
