pipeline {
    agent any
 
    stages {
       stage('Build') {
            steps {
                sh 'mvn -B clean verify'
                echo "Build Done"
            }
        }
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
}      
}
