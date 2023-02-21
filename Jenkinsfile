pipeline {
    agent any
 
    stages {
        stage('Checkout Code') {
            steps {
                echo 'Checkout Completed'
            }
        }
       stage('Build') {
            steps {
                sh 'mvn -B clean verify'
                echo 'Build Completed'
            }
        }
}      
}
