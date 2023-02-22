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
    post {
       always {
          junit(
        allowEmptyResults: true,
        testResults: '*/test-reports/.xml'
      )
      }
   } 
}
