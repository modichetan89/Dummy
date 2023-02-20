pipeline {
    agent any
 
    stages {
       stage('Example Build') {
            steps {
                sh 'mvn -B clean verify'
            }
        }
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
}      
}
