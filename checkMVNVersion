pipeline {
    agent any
    tools {
        maven 'MAVEN_HOME' 
    }
    stages {
        stage('Example') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
