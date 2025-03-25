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
                rm -rf $VIRTUAL_ENV  # Hapus venv jika sudah ada
                python3 -m venv $VIRTUAL_ENV
                bash -c "source $VIRTUAL_ENV/bin/activate && pip install --upgrade pip && pip install -r requirements.txt"
                '''
            }
        }
        stage('Run Migrations') {
            steps {
                sh '''
                bash -c "source $VIRTUAL_ENV/bin/activate && python manage.py migrate"
                '''
            }
        }
        stage('Run Tests') {
            steps {
                sh '''
                bash -c "source $VIRTUAL_ENV/bin/activate && python manage.py test --verbosity=2"
                '''
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying Django application...'
                echo 'Push into server'
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
