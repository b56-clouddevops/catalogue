pipeline {
    agent any
    stages {
        stage('Lint Checks'){
            steps {
                sh "whoami"
                sh "echo ***** Starting Style Checks *****"
                sh "npm install jslint"
                sh "ls -ltr node_modules/jslist/bin"
                sh "node_modules/jslint/bin/jslist.js server.js"
                sh "echo ***** Style Checks Are Completed *****"
            }
        }
        stage('Static Code Analysis') {
            steps {
                sh "echo Starting Static Code Analysis"
            }
        }
    }
}

