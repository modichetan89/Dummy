pipeline {
    agent any
 
    stages {
       stage('Build') {
            steps {
                sh 'mvn -B clean verify'
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
