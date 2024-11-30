pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo "1"
                echo "2" >> 2.txt
                echo 'Hello, World!'
            }
        }

        stage("goodbye"){
            steps{
                echo "good bye!"
            }
        }
    }  

    post {
        always {
            echo 'Pipeline execution completed!'
        }
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
