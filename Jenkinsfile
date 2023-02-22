pipeline {
    agent any
 
    stages {
       stage('Build') {
            steps {
                echo 'Build Start'
                bat "mvn -D clean test"
                echo 'Build Completed'
            }
        }
    }   
}
