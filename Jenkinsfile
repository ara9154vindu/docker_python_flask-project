pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                git branch: 'main', url: 'https://github.com/ara9154vindu/docker_python_flask-project.git'
            }
        }
        stage('pip') {
            steps {
                sh 'pip install requirements.txt'
            }
        }
        stage('python') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
