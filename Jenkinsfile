pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }

           stage('Deploy Static Site') {
                steps {
                    sh '''
                    sudo cp -r /var/lib/jenkins/workspace/MY-DATA_PIPELINE/* /var/www/html/
                    '''
                }
            }
    }
}