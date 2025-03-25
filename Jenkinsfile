pipeline {
    agent any
    environment {
        VIRTUAL_ENV = 'venv'
        DJANGO_SETTINGS_MODULE = 'myproject.settings'
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/rushiaremka/django-prak-3.git'
            }
        }
        stage('Setup Virtual Environment') {
            steps {
                sh '''
                python3 -m venv $VIRTUAL_ENV
                source $VIRTUAL_ENV/bin/activate
                pip install -r requirements.txt
                '''
            }
        }
        stage('Run Migrations') {
            steps {
                sh '''
                source $VIRTUAL_ENV/bin/activate
                python manage.py migrate
                '''
            }
        }
        stage('Run Tests') {
            steps {
                sh '''
                source $VIRTUAL_ENV/bin/activate
                python manage.py test --verbosity=2
                '''
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying Django application...'
                echo 'push into server'
            }
        }
    }
    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
