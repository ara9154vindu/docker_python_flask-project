pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                git branch: 'main', url: 'https://github.com/ara9154vindu/docker_python_flask-project.git'
            }
        }
        stage('python') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
