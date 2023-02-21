pipeline {
    agent any
 
    stages {
       stage('Build') {
            steps {
                echo "Build started"
                sh 'mvn -B clean verify'
                echo "Build Done"
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
