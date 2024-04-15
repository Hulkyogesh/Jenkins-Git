pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hi Welcome to Pipeline Job Example'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'Build started on echo $date', subject: 'Build started on echo $date', to: 'yogeshbarshi0@gmail.com'
        }
    }
}
