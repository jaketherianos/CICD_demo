pipeline {
    agent { docker { image 'python:3.10.1-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'ls'
                sh 'pwd'
                sh 'python print.py'
                sh """#!/bin/bash
                  echo ${env.JOB_NAME}
               """
            }
        }
    }
}
