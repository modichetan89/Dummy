pipeline {
    agent any
 
    stages {
       stage('Build') {
            steps {
                echo 'Build Start'
                sh 'mvn -B clean verify'
                echo 'Build Completed'
            }
        }
}      
}
