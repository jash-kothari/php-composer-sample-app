#!/usr/bin/env groovy
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "php -v"
                sh "composer -V"
                sh "composer install --ignore-platform-reqs --no-interaction --no-plugins --no-scripts --prefer-dist"
                sh "cp -r * /var/www/html"
            }
        }
        stage('Deploy') {
            steps {
                sh "cp -r * /var/www/html"
            }
        }
        stage('Done') {
            steps {
                echo "Done"
            }
        }
    }
}
