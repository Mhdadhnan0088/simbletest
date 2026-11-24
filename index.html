
pipeline {
    agent none

    stages {
        stage('build') {
            agent {
                label 'build-node'
            }

            steps {
                deleteDir()

                sh '''
                    git clone https://github.com/adhnan0088/adhnan.git
                    ls -la
                '''

                stash name: 'webpage', includes: 'adhnan/**'
            }
        }

        stage('deploy') {
            agent {
                label 'deploy-node'
            }

            steps {
                deleteDir()

                unstash 'webpage'

                sh '''
                    sudo rm -rf /var/www/html/*
                    sudo cp -r adhnan/* /var/www/html/
                    ls -la /var/www/html/
                '''
            }
        }
    }
}
