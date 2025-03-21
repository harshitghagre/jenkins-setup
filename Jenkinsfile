pipleline{
    agent any
    stages {
        stage('Checkout'){
            steps {
                git url: 'https://github.com/harshitghagre/jenkins-setup.git', branch 'main'
            }
        }
        stage('Build'){
            steps{
                sh 'python3 hello.py'
            }
        }
    }
    post{
        always{
            echo 'Pipeline completed!'
        }
    }
}
