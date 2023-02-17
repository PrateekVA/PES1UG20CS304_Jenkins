pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 build job: 'PES1UG20CS304-1', wait: false
                 echo 'Build by CS304 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                ech 'Test by CS304 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by CS304 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
