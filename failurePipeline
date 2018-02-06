pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                echo "hello"
            }
        }
    }
     post {
        always {
            echo "hello again"
            sh('buidl.sh')
        }
    success {
      mail(from: "heenashree2010@gmail.com", 
           to: "heenashree2015@gmail.com", 
           subject: "That build passed.",
           body: "Nothing to see here")
        }
    failure {
      mail(from: "heenashree2010@gmail.com", 
           to: "heenashree2015@gmail.com", 
           subject: "That build failed.",
           body: "Nothing to see here")
        }
 
    }
}
