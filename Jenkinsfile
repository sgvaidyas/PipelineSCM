pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App'
            }
        }
        stage('Test') {
            steps {
                echo 'Test App'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
    }
    post{
        always
        {
                emailext body: 'and a summary goes here', subject: 'this is just  a pipeline msg', to: 'excelincredible@gmail.com'
        }
    }
}
