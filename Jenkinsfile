#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: 'Shivakumar',
    projectUrlStr: 'https://github.com/My-NewOrganization/NewYork.git'],
    pipelineTriggers([
      upstream(
      threshold: 'SUCCESS',
      upstreamProjects: 'https://github.com/My-NewOrganization/Massachusetts.git'
      )
    ])
])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}
