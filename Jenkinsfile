pipeline {
    agent {
        label "ws"
    }
    stages {
        stage('Lint Checks'){
            steps {
                sh "echo ***** Starting Style Checks *****"
                sh "/home/centos/node_modules/jslint/bin/jslist.js server.js"
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