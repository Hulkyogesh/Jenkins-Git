pipeline {
    agent any

    echo "the job name is ${env.JOB_NAME}"
    echo "the build number is ${env.BUILD_NUMBER}"
    echo "The node name is ${env.NODE_NAME}"

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
