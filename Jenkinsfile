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
        stage('Publish Junit Results') {
            steps {
                echo 'Publishing junit results'
                junit skipMarkingBuildUnstable: true, testResults: 'xmlReport/output.xml'
            }
        }
}      
}
