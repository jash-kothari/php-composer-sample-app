#!/usr/bin/env groovy
pipeline {
    agent any
    stages {
        stage('stage one') {
            steps {
                sh "php -v"
            }
        }
        stage('stage two') {
            steps {
                sh "composer -V"
            }
        }
        stage('stage two') {
            steps {
                sh "composer -V"
            }
        }
        stage('stage three') {
            steps {
                sh "composer install --ignore-platform-reqs --no-interaction --no-plugins --no-scripts --prefer-dist"
            }
        }
        stage('stage four') {
            steps {
                sh "cp -r * /var/www/html"
            }
        }
        stage('stage four') {
            steps {
                echo "Done"
            }
        }
    }
}
