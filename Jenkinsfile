// pwd: /var/jenkins_home/workspace/declerative-pipeline

pipeline {
    // triggers {
    //     cron '* * * * *'
    // }
    agent any

    stages {
        stage('Clone') {
            environment {
                JOB_TIME = sh (returnStdout: true, script: "date '+%A %W %Y %X'").trim()
            }
            steps {
                echo 'Cloning stage $JOB_TIME'

		dir('/var/jenkins_home/workspace/declerative-pipeline') {
                    script {
			sh 'rm -f *.*'
			sh 'rm -rf jenkins-startup'
                        sh 'git clone https://github.com/shiloyuval/jenkins-startup.git'	                      
                    }
                }  
            }
        }

        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}